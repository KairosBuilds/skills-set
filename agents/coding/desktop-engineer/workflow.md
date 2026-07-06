# Workflow — Desktop Engineer

## Standard Desktop App Workflow

### Step 1: Framework Selection
- Evaluate requirements vs framework capabilities
- Choose Electron for web-based UI or Tauri for native
- Choose WPF/WinForms for Windows-native apps

### Step 2: Project Setup
- Initialize project with build tooling
- Configure TypeScript, linting, testing
- Set up main/renderer process separation
- Configure native module compilation

### Step 3: Core Implementation
- Implement main process (Electron) or Rust backend (Tauri)
- Set up IPC communication
- Implement file system access
- Implement system tray and notifications
- Configure window management

### Step 4: UI Implementation
- Build renderer with React/Vue
- Implement desktop-specific UI patterns
- Add keyboard shortcuts and menus
- Implement drag-and-drop

### Step 5: Packaging
- Configure electron-builder or tauri-bundler
- Set up code signing
- Create installers for each platform
- Configure auto-updates