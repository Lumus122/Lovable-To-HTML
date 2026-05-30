# Lovable-To-HTML

Lovable-To-HTML is a Python tool for converting a Lovable project export, extracted from a ZIP archive, into a static HTML website.  
It is designed to help turn a Lovable / Vite project into a final HTML build while keeping the original structure and behavior as close as possible.

## What is Lovable-To-HTML?

Lovable-To-HTML is an AI-built Python converter for Lovable projects.  
It works on an already extracted project folder, detects the project structure, installs dependencies, updates the required files, and generates a ready-to-use HTML output.

This tool is useful when you need to export a Lovable project to HTML, create a static website build, or automate the conversion of a Lovable/Vite app into a single deployable result.

## Features

- Converts an extracted Lovable ZIP archive into HTML
- Detects whether `bun` is available and falls back to `npm` when needed
- Installs project dependencies automatically
- Installs `vite-plugin-singlefile`
- Updates `vite.config.ts`
- Updates `src/routes/__root.tsx`
- Updates `src/router.tsx`
- Creates `src/main.tsx`
- Creates `index.html`
- Builds the project
- Copies the generated `dist/index.html` to the Desktop

## Requirements

- Windows
- Python installed
- Node.js or Bun installed
- A Lovable / Vite project already extracted into a folder
- The script must be placed inside the extracted project folder
- Administrator privileges are recommended

## How to Use

1. Extract the ZIP archive into a folder.
2. Place `Lovable-To-HTML` inside that extracted folder.
3. Open Command Prompt as Administrator.
4. Go to the folder that contains both the extracted project and the script.
5. Run the Python script.
6. Follow the on-screen instructions.

## How It Works

1. The script checks the current working directory.
2. It verifies that a `package.json` file exists.
3. It installs dependencies.
4. It updates the project files needed for the HTML export.
5. It builds the project.
6. It exports the final HTML file.
7. It copies `dist/index.html` to the Desktop.

## Output

The final output is an HTML version of the project, generated in the `dist` folder and copied to the Desktop.

Depending on the system configuration, the Desktop path may be:

- Local Desktop
- OneDrive Desktop

## Notes

- The tool requires a valid project structure with `package.json`.
- If `package.json` is missing, the process stops.
- The output depends on the original Lovable/Vite project structure.
- Some projects may require manual adjustments after conversion.

## Disclaimer

This project is provided for educational and experimental purposes only. Use it at your own risk.  
The author is not responsible for any loss, damage, or unexpected behavior resulting from its use.
