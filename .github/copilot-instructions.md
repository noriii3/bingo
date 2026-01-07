# Copilot Instructions

Before committing code changes:
- [ ] `npm run lint` passes
- [ ] `npm run build` succeeds
- [ ] `npm test` passes


## Architecture

**State separation**: `useBingoGame` hook wraps pure functions from `bingoLogic.ts` (zero React deps). Components receive `board`, `winningSquareIds`, callbacks.

**3-state machine**: `GameState = 'start' | 'playing' | 'bingo'`. App.tsx conditionally renders StartScreen OR GameScreen+BingoModal.

## Critical Rules

- `BOARD_SIZE = 5`, `CENTER_INDEX = 12` in `bingoLogic.ts` - never hardcode
- Free space at index 12, always marked, immutable
- Keep 24+ questions in `questions.ts` (board needs 24 after shuffle)
- Win = 12 lines: 5 rows + 5 cols + 2 diagonals

## localStorage

Versioned persistence in `useBingoGame.ts` - bump `STORAGE_VERSION` to invalidate corrupt data. Use `validateStoredData()` and `typeof window === 'undefined'` guards.

## Tailwind v4

Define tokens in `@theme` block in `index.css` (no config file). Use `bg-marked`, `border-marked-border`. Native opacity: `bg-black/50`. State-based classes: `square.isMarked ? 'bg-marked' : 'bg-white'`.

## Testing

Vitest + jsdom. Mock `Math.random` for shuffle tests. Test pure functions in `bingoLogic.test.ts`, not components.
