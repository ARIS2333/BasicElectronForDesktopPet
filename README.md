# Electron Desktop Pet

A simple always-on-top draggable desktop pet with transparent background using Electron

## Features
- 🧲 Always stays on top of other windows
- ✨ Transparent background
- 🖱️ Draggable red circular pet
- 🚀 Minimal Electron setup

## Project Structure
```bash
├── main.js          # Electron main process
├── index.html       # UI with draggable element
└── package.json     # Project configuration
```

## Setup
1. Initialize project
```bash
npm init -y
```

2. Install Electron
```bash
npm install electron --save-dev
```

3. Add start script to package.json
```json
"scripts": {
  "start": "electron ."
}
```

## Usage
```bash
npm start
```

## Controls
- Drag red circle to move
- Press `Cmd+Q` (macOS) / `Alt+F4` (Windows) to quit

## Customization
- Modify `index.html` to change pet appearance
- Adjust window size in `main.js` constructor