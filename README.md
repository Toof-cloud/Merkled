# Merkled - Digital File Preservation Tool 🔒

A Chrome extension for file preservation using Merkle Tree cryptographic hashing.

## Features

- **Seal**: Hash files/folders using SHA-256 Merkle Trees
- **Verify**: Re-upload to detect any tampering
- **Export**: Save manifests as JSON or PDF
- **Offline**: All processing happens locally in browser

## Running in Browser (Development Mode)

To run the application in your browser:

```bash
# 1. Navigate to frontend directory
cd frontend

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
```

The app will open at `http://localhost:5173` in your default browser.

## Building as Chrome Extension

To use as a Chrome/Edge extension:

```bash
# 1. Navigate to frontend directory
cd frontend

# 2. Install dependencies (if not already done)
npm install

# 3. Build the extension
npm run build:extension

# 4. Load in Chrome/Edge
#    - Open chrome://extensions/ (or edge://extensions/)
#    - Enable "Developer mode" toggle (top right)
#    - Click "Load unpacked"
#    - Select the frontend/dist folder
```

## Usage

1. Click the extension icon (or open the browser app)
2. Drag & drop a folder or click "Select Folder"
3. Click "Generate Merkle Root"
4. Export manifest (JSON/PDF) for proof

## Development Commands

```bash
npm run dev              # Start dev server at localhost:5173
npm run build            # Build for production
npm run build:extension  # Build for Chrome/Edge extension
npm run preview          # Preview production build
```

## Project Structure

```
frontend/
├── src/app/components/  # UI components
├── src/utils/           # Merkle Tree logic
├── public/              # Extension manifest & icons
└── dist/                # Built extension (load this in Chrome)
```

---

MIT License
  
