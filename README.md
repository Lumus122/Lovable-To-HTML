# Lovable-To-HTML
Lovable To HTML is an AI-built Python tool that converts an extracted ZIP Lovable archive into a fully functional HTML website, preserving the original structure and features as closely as possible.

## Overview

Lovable To HTML is designed to be placed inside the extracted project folder. The tool checks the current working directory, verifies that a `package.json` file is present, installs the required dependencies, updates the project files, and generates a final HTML build.

The first part of the process may take anywhere from a few seconds to several minutes, depending on the size and complexity of the project.

## Requirements

- Windows
- Python installed
- Node.js or Bun installed
- A Lovable/Vite project already extracted into a folder
- The script must be placed inside that extracted project folder
- Administrator privileges recommended

## How to Use

1. Extract the ZIP archive into a folder.
2. Move `Lovable To HTML` into that extracted folder.
3. Open **Command Prompt as Administrator**.
4. Navigate to the folder that contains the extracted project and the script.
5. Run the Python script.
6. Follow the on-screen instructions.

## What the Tool Does

- Detects whether `bun` is available, otherwise falls back to `npm`
- Runs dependency installation
- Installs `vite-plugin-singlefile`
- Updates `vite.config.ts`
- Updates `src/routes/__root.tsx`
- Updates `src/router.tsx`
- Creates `src/main.tsx`
- Creates `index.html`
- Builds the project
- Opens and copies the generated `dist/index.html` to the Desktop

## Notes

- The tool requires a valid project structure with `package.json`.
- If `package.json` is missing, the process stops.
- The final HTML output may be copied either to the local Desktop or to the OneDrive Desktop, depending on the system configuration.

## Disclaimer

This project is provided for educational and experimental purposes only. Use it at your own risk. The author is not responsible for any loss, damage, or unexpected behavior resulting from its use.
