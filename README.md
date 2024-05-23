# electron-gpt

Electron desktop chatbot demo using the OpenAI API.

## About

This repo is a compact Electron Forge application that wraps a local chat UI around OpenAI-powered responses. The project is intentionally small and works well as a desktop-app portfolio sample.

## Key Features

- Electron main, preload, and renderer separation
- OpenAI-powered chat completions
- Tailwind styling for the UI
- Packaged app workflow through Electron Forge

## Architecture

- `main.js` boots Electron and configures the app window
- `preload.js` exposes safe bridge behavior to the renderer
- `renderer.js` handles the chat UI
- `database.js` stores local app data

## Tech Stack

- Electron
- Node.js
- OpenAI SDK
- Tailwind CSS

## Prerequisites

- Node.js
- OpenAI API key

## Installation

```bash
npm install
```

## Configuration

- `OPENAI_API_KEY`

## How to Run

```bash
npm start
npm run package
npm run make
```

## Example Usage

- Launch the desktop app and send a prompt in the chat UI

## Project Structure

- `main.js` - Electron main process
- `preload.js` - preload bridge
- `renderer.js` - UI logic
- `assets/` - icons and screenshots

## Current Status

Functional demo, but it still reads like a prototype rather than a hardened desktop product.

## Limitations

- Requires an OpenAI key
- No tests

## License

The repository includes `LICENSE.md` with a CC0 1.0 Universal license.
