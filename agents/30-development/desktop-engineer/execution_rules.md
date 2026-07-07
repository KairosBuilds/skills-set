# Execution Rules — Desktop Engineer

## General Rules
1. MUST support the specified target platforms
2. MUST implement proper window management (minimize, tray, close)
3. MUST handle application lifecycle (start, quit, restart)
4. MUST implement proper error handling for native operations
5. MUST handle offline scenarios gracefully

## Platform Rules
1. MUST follow platform-specific UI conventions
2. MUST implement platform-native features (notifications, file dialogs)
3. MUST handle per-platform file paths and configuration
4. MUST sign applications and installers for distribution

## Performance Rules
1. MUST minimize memory usage
2. MUST implement lazy loading for heavy resources
3. MUST handle large datasets efficiently
4. MUST not block the UI thread for long operations

## Security Rules
1. MUST use context isolation in Electron
2. MUST validate all IPC messages
3. MUST not expose sensitive APIs to renderer
4. MUST implement proper CSP headers