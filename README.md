
# React + TypeScript Chrome Extension Template

A minimal template for creating Chrome extensions using React, TypeScript, and [shadcn/ui](https://ui.shadcn.dev/). This template includes a simple reload script for streamlining development.

## Features

- **React + TypeScript**: Build your extension using the modern React framework with full TypeScript support.
- **shadcn/ui**: Pre-configured with shadcn/ui components for a consistent and customizable design system.
- **Automatic Reload**: Includes a simple reload script to streamline development by automatically reloading the extension after building.

## Getting Started

Follow these steps to set up and develop your Chrome extension:

### 1. Clone the Repository

```bash/Users/ericstratigakis/Downloads/README.md
git clone https://github.com/your-username/react-ts-chrome-extension-template.git
cd react-ts-chrome-extension-template
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Develop Your Extension

Run the development server:

```bash
npm run dev
```

Edit the code in the `src/` directory. The `vite` development server will reload the app automatically for changes.

### 4. Build the Extension

To build the production-ready extension:

```bash
npm run build
```

The build output will be in the `dist/` directory.

### 5. Reload Extension Automatically (Optional)

During development, you can use the `reload-extension.js` script to reload the extension in Chrome after each build:

```bash
npm run reload
```

Ensure that Chrome is running with remote debugging enabled. Start Chrome with the following command:

```bash
google-chrome --remote-debugging-port=9222
```

For macOS:

```bash
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --remote-debugging-port=9222
```

### 6. Load the Extension in Chrome

1. Open Chrome and navigate to `chrome://extensions/`.
2. Enable "Developer mode" in the top-right corner.
3. Click "Load unpacked" and select the `dist/` directory.

Your extension is now ready to use!

## File Structure

```
react-ts-chrome-extension-template/
├── public/             # Static files (e.g., icons)
├── src/                # Application source code
│   ├── App.tsx         # Main React component
│   ├── background.ts   # Background script
│   ├── content.ts      # Content script
│   ├── index.tsx       # Entry point for React
├── dist/               # Build output
├── manifest.json       # Chrome extension manifest
├── vite.config.ts      # Vite configuration
├── reload-extension.js # Script for reloading the extension
```

## Scripts

- `npm run dev`: Start the development server.
- `npm run build`: Build the extension for production.
- `npm run reload`: Reload the extension in Chrome.

## Dependencies

- [React](https://reactjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [shadcn/ui](https://ui.shadcn.dev/)

## License

This project is licensed under the [MIT License](LICENSE).

---

Happy coding!
