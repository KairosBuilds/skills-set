# Examples — Desktop Engineer

## Example: Markdown Editor App
**Requirements:** Cross-platform markdown editor with file system access

**Stack:** Electron + React + TypeScript

**Implementation:**
1. Main process: file I/O, window management, menu bar
2. Renderer: React editor component with CodeMirror
3. Features: open/save files, preview, syntax highlighting
4. Native: file dialogs, system tray, auto-update
5. Packaging: electron-builder for Windows/macOS/Linux

**Output:** Complete desktop markdown editor application