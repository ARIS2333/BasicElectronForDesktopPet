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


## Packaging (macOS DMG)

### 1. Install Packager
```bash
npm install electron-packager --save-dev
```

### 2. Add Build Script to package.json
```json
"scripts": {
  "start": "electron .",
  "build": "electron-packager . --platform=darwin --format=DMG --electron-version=38.1.0"
}
```

### 3. Run Build Command
```bash
npm run build
```

### 4. Output Location
The DMG file will be created in:
```bash
/Users/alice/Code/electronTest/electronTest-darwin-arm64
```

## Common Issues

### ❌ Electron Version Error
**Error Message:**
```
Unable to determine Electron version. Please specify an Electron version
```

**Solution:**
Always manually specify the version in your build command:
```bash
--electron-version=38.1.0
```

### 📦 Dependency Warnings
You may see warnings about deprecated packages - these are non-critical and won't affect the basic functionality of your DMG build.
