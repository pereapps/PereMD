# Changelog

All notable changes to **PereMD** are documented in this file.

## [0.5.0] - 2026-11-21

### Added
- **30-Language Global Localization:** Added full UI localization in English (default) plus 29 additional languages (`Tiếng Việt`, `日本語`, `한국어`, `简体中文`, `繁體中文`, `Français`, `Deutsch`, `Español`, `Português (Brasil)`, `Português`, `Italiano`, `Nederlands`, `Русский`, `Українська`, `Polski`, `Türkçe`, `Bahasa Indonesia`, `Bahasa Melayu`, `ไทย`, `हिन्दी`, `Čeština`, `Slovenčina`, `Svenska`, `Dansk`, `Norsk`, `Suomi`, `Magyar`, `Ελληνικά`, `Română`) across all menus, tooltips, dialogs, Mermaid canvas overlays, and built-in extensions, with fast on-demand loading and instant switching in Settings.
- **Windows Installer Language Sync:** Select your preferred setup language directly in the Windows installer; PereMD automatically opens in that language on first launch while preserving existing language preferences across silent updates.
- **Mermaid Visual Editor Overhaul:** Redesigned the Visual Editor with a unified compact toolbar, two-row SVG connection palette, categorized 30-shape Flowchart picker (`Basic` / `Process` / `Technical`), Fill and Border color pickers across 18 swatches, node duplication, edge selection glow, Undo/Redo history, edge curve routing, diagram theme presets, quick-insert canvas rail, dot-grid background, live zoom controls, keyboard shortcuts (`Del`, `F2`/`Enter`, `Ctrl+D`, `Space+Drag`, layered `Esc`), and an interactive `?` user guide.
- **One-Click Simple & Colorful Diagram Palettes:** Cycle between clean monochrome **Simple** styling and curated **Colorful** palettes across all 30 Mermaid diagram types, with newly added nodes and objects automatically inheriting your active diagram palette.

### Improved & Fixed
- **Adaptive Multilingual Layout:** Standardized sidebar button sizing and automatically adapted default sidebar width for longer languages while preventing top toolbar label collisions and narrow inline Mermaid toolbar clipping.
- **Window Dragging:** Fixed an issue where the PereMD window could not be dragged to a new position in windowed mode.
- **Inline Diagram Text Editing:** Double-clicking a diagram node in Edit mode opens a spacious auto-resizing text editor (with multiline support), ignores accidental double-clicks in Read mode, and keeps node action toolbars inside viewport bounds.
- **Fullscreen Diagram Sync:** Kept diagram scale, aspect ratio, and selection overlays aligned when opening fullscreen after inline edits or switching between Visual and Code modes.

---

## [0.4.0] - 2026-11-20

### Added
- **Built-in Extensions Suite:** Enable four opt-in productivity extensions from the new **Extensions** tab in Settings (all off by default):
  - **Git Control:** Inspect changes, view inline diffs, stage/discard edits, switch branches, and commit, pull, or push right from the sidebar.
  - **Workspace Search:** Search Markdown files across your active folder or repository with instant context snippets, visible Mermaid label matching, and click-to-jump navigation.
  - **Document Templates:** Create files faster using built-in SRS, ADR, Meeting Notes, Release Changelog, and Project README blueprints or save your own custom templates.
  - **Export Pro:** Export formatted documents and Mermaid diagrams to PDF, Word (`.docx`), or offline HTML using Corporate, Technical, or Minimal presets with optional cover pages, TOC, headers/page numbers, and automatic landscape framing for wide tables.
- **Tab Management & Unsaved Protection:** Right-click any tab for **Close Tab**, **Close Other Tabs**, **Close Tabs to the Right**, and **Close All Tabs**, backed by a batch unsaved-changes confirmation dialog (`Save All & Close`, `Close Without Saving`).
- **Session & Layout Memory:** Reopen tabs from your previous session on launch (configurable in Settings) and preserve Outline (Table of Contents) visibility and maximized window state across restarts and fullscreen (`F11`).
- **Document Status Footer:** View your active save folder (click to reveal in Explorer), detected Git branch badge, total lines, and character length in the footer bar.
- **Customizable Markdown File Icons:** Pick from 4 `.md` icon styles (**Classic Document**, **Document MD**, **Modern Markdown**, **Code Markdown**) in Settings for both PereMD tabs/lists and Windows Explorer file associations.

### Improved & Fixed
- **Clearer Toolbar & Display Controls:** Replaced `Edit`/`Done` with a `Read | Edit` mode switch alongside a primary **Save** action for unsaved changes, consolidated font size, page width, and dual layout controls into the **Aa Display Options** popover, and fixed font-size scaling across headings, tables, code blocks, and Raw panes.
- **In-Document Diagram Search (`Ctrl+F`):** Search and highlight matching text directly inside rendered Mermaid diagrams alongside regular prose, with typing-pause debouncing and TOC-safe positioning.
- **Smoother Preview Editing:** Clicking empty space below Mermaid diagrams, headings, or code blocks in Preview Edit mode now creates and focuses a new paragraph ready to type, with `Ctrl+N` / `Ctrl+P` fallback navigation in the `/` Slash menu.
- **Refined Library Sidebar, New File & Settings:** Streamlined the Library sidebar panel for clearer file browsing, kept the `.md` extension locked in the New File dialog, and redesigned **Settings & About** into a cleaner two-column layout.
- **Export & Bookmark Fixes:** Fixed Mermaid **Export SVG** and **Export PNG** buttons to save directly via the desktop file dialog, and fixed the **Add to Favorites** modal defaulting the Root folder to unchecked when bookmarking new files.

---

## [0.3.0] - 2026-11-18

### Added
- **Full Mermaid Editor & 30 Diagram Types:** Write, validate, and preview 30 Mermaid diagram types with syntax highlighting, context-aware autocomplete (including inside ```` ```mermaid ```` blocks in Raw view), live preview, and a searchable 30-template picker.
- **Visual Drag-and-Drop Canvas (9 Diagram Types):** Visually edit **Flowchart, Swimlanes, ER, State, Mindmap, Sequence, Class, C4, and Architecture** diagrams directly on the canvas—add or remove nodes, drag handles to connect relationships, double-click labels or arrows to edit inline, and customize line thickness and arrowhead styles while preserving comments and frontmatter.
- **Diagram Export:** Export any Mermaid diagram directly to **SVG** or high-resolution **PNG (2x)**.
- **Privacy-First Update Controls:** Added an **Automatically check for updates on startup** toggle in Settings (off by default); manual update checks remain available anytime.

### Improved & Fixed
- **Slash Command Menu:** Improved suggestion ranking (e.g., `/me` prioritizes *Mermaid Diagram* first) and fixed `ArrowUp`/`ArrowDown`/`Enter`/`Esc` keyboard navigation.
- **Mermaid Viewport & Display:** Improved diagram scrolling and scaling, plus smoother multi-monitor window sizing and `F11` fullscreen behavior.

---

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
