# PereMD — Minimalist Notion-style Markdown Reader

**PereMD** is a lightweight, fast local Markdown reader for Windows, combining a clean **Termius-inspired** workspace layout with **Notion-style** typography and reading experience.

> [!NOTE]
> PereMD is **closed-source freeware** that runs **100% offline on your device**, with zero analytics or telemetry.

---

## Key Features

- **3 Viewing Modes:** `Raw` (CodeMirror 6), `Preview` (Notion-style typography), and `Dual` (50/50 side-by-side split view with smooth resizable divider).
- **Content-Aware Two-Way Sync Scroll:** Synchronizes Raw and Preview panes by document block structure (`data-block-id`) rather than naive scroll percentage, keeping large tables and diagrams aligned.
- **Offline Mermaid Diagrams (`Pele`):** Built-in SVG rendering with zero internet dependency, zoom controls (`Ctrl + Mouse Wheel`), fullscreen overlay, and source copy.
- **Convenient Document Management:** Multi-tab support, Recent Files modal with search and pagination, hierarchical Favorites folders with drag-and-drop, quick `New` file creation, and context menu actions (`Copy Filename`, `Copy Path`, `Open File Location`, `Rename`, `Hide`, `Delete`).
- **Privacy by Default:** Blocks external remote images in Markdown documents until you explicitly allow them; stores workspace metadata locally in SQLite (`%APPDATA%\com.peremd.reader\peremd.db`).
- **Built-in Auto-Updater:** Check for and install signed updates directly from `Settings → General & About`.

---

## Download & Installation (Windows x64)

Download the latest release from **[GitHub Releases](https://github.com/pereapps/PereMD/releases/latest)**:

- **`PereMD_<version>_x64-setup.exe`**: Standard NSIS installer (registers `.md` / `.markdown` file associations and supports automatic updates).
- **`PereMD_<version>_x64_Portable.zip`**: Portable archive—extract and run without installation.

*(Please verify the `SHA-256` checksum included in each Release's notes to ensure file integrity.)*

---

## FAQ & Bug Reports

- **Why does Windows SmartScreen show a warning on first launch?**
  Early freeware releases are not yet signed with a commercial Authenticode EV certificate. You can verify the `SHA-256` checksum against the Release page and click *More info → Run anyway*, or use the `Portable.zip` package.
- **Feedback & Bug Reports:** Please open an issue in **[GitHub Issues](https://github.com/pereapps/PereMD/issues)** with your PereMD version and steps to reproduce.
