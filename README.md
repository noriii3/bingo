<div align="center">

# 🎉 Soc Ops

### Break the Ice with Social Bingo

*The fun, interactive way to help people connect at mixers, team events, and gatherings*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Built with React](https://img.shields.io/badge/React-19-61dafb.svg)](https://react.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.0-38bdf8.svg)](https://tailwindcss.com/)

[🎮 Live Demo](https://noriii3.github.io/bingo/) • [📖 Lab Guide](.lab/GUIDE.md) • [🤝 Contributing](CONTRIBUTING.md)

</div>

---

## 🎯 What is Soc Ops?

Soc Ops is a **social bingo game** designed to transform awkward mixer moments into engaging conversations. Players mingle and find people who match fun prompts like "has lived in another country" or "speaks more than 2 languages"—then mark their bingo board. First to get 5 in a row wins! 🏆

Perfect for:
- 👥 Team building events
- 🎓 Networking mixers
- 🎊 Social gatherings
- 🏢 Onboarding new team members
- 🎤 Conference icebreakers

## ✨ Features

- **🎲 Randomized Boards** – Every game generates a unique 5×5 grid from your question pool
- **💾 Auto-Save Progress** – Pick up right where you left off with localStorage persistence
- **📱 Mobile Friendly** – Responsive design works perfectly on phones and tablets
- **🎨 Modern UI** – Built with React 19 and Tailwind CSS v4
- **⚡ Lightning Fast** – Instant loading with Vite build system
- **🔒 Privacy First** – No data collection, runs entirely in your browser

## 🚀 Quick Start

### Prerequisites

- [Node.js 22+](https://nodejs.org/)

### Run Locally

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Visit `http://localhost:5173` to play! 🎮

### Build for Production

```bash
npm run build
```

The optimized build outputs to `/dist` and automatically deploys to GitHub Pages on push to `main`.

## 🎮 How to Play

1. **Start the Game** – Launch the app and click "Start Game"
2. **Mingle & Mark** – Talk to people at your event and find those who match the prompts
3. **Get 5 in a Row** – Mark squares as you find matches (horizontal, vertical, or diagonal)
4. **Shout BINGO!** – Be the first to complete a line and celebrate! 🎊

The center square is a **FREE SPACE** to get you started!

## 🛠️ Customization

Want to personalize the questions for your event? It's easy!

1. Edit the prompts in [`src/data/questions.ts`](src/data/questions.ts)
2. Add at least 24 unique questions (the game needs 24 + 1 free space)
3. Rebuild and deploy

💡 **Tip:** See the [Lab Guide](.lab/GUIDE.md) for detailed customization instructions.

## 🏗️ Tech Stack

- **React 19** – Modern UI with hooks and functional components
- **TypeScript** – Type-safe code for reliability
- **Tailwind CSS v4** – Utility-first styling with CSS-first configuration
- **Vite** – Next-gen build tool for blazing fast development
- **Vitest** – Lightning-fast unit testing

## 📚 Documentation

- [Lab Guide](.lab/GUIDE.md) – Setup and customization walkthrough
- [Contributing Guidelines](CONTRIBUTING.md) – How to contribute
- [Code of Conduct](CODE_OF_CONDUCT.md) – Community standards
- [Security Policy](SECURITY.md) – Report vulnerabilities
- [Support](SUPPORT.md) – Get help

## 🤝 Contributing

Contributions are welcome! Whether it's:
- 🐛 Bug fixes
- ✨ New features
- 📝 Documentation improvements
- 🎨 UI/UX enhancements

Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started.

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

## 💖 Acknowledgments

Created by [Harald Kirschner](https://github.com/noriii3) with love for bringing people together.

---

<div align="center">

**[⭐ Star this repo](https://github.com/noriii3/bingo)** if you find it useful!

Made with ❤️ and React

</div>
