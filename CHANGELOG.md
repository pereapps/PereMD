# Changelog

All notable changes to **PereMD** are documented in this file.

## [0.2.0] - 2026-11-17

### Added
- **Built-in Auto-Updater:** Check for, download, and install signed updates from GitHub Releases directly inside `Settings → General & About`.
- **Licenses & Privacy Viewer:** Added a dedicated Settings view displaying local-only privacy guarantees and third-party notices (`THIRD-PARTY-LICENSES.txt`).
- **Multi-Tab Support & Recent Files Modal:** Open multiple documents in tabs, browse recent files with search and pagination, and receive prompts when an open file changes on disk.
- **Enhanced File Management:** Added the `New` Markdown file creation flow and right-click context menu actions (`Copy Filename`, `Copy Path`, `Open File Location`, `Rename`, `Hide`, `Delete`).
- **Unified Custom Titlebar:** Integrated a compact custom titlebar with full Windows window controls.

### Improved & Fixed
- Improved multi-monitor window dragging, work-area bounds clamping on unmaximize, and F11 fullscreen state persistence.
- Disabled unwanted default browser context menus, DevTools shortcuts, and accelerator keys in release builds.

---

## [0.1.0] - 2026-11-13

### Initial Release
- Launched local Windows x64 Markdown reader built with Tauri 2 (Rust) and Svelte 5.
- Three viewing modes (`Raw` via CodeMirror 6, `Preview` with Notion-style typography, `Dual` 50/50 split) with content-aware two-way sync scroll.
- Offline Mermaid diagram rendering via `Pele 1.13.0` with zoom, fullscreen overlay, and source copy.
- Favorites & virtual folder organization stored locally in SQLite (`%APPDATA%\com.peremd.reader\peremd.db`).
- HTML sanitization with `ammonia` (blocking `<script>`, `<iframe>`, `javascript:`, and inline event handlers) plus default blocking of remote images.
