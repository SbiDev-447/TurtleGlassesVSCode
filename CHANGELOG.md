# Changelog

## [0.2.4] - 2026-09-17

### Fixed
- Dark theme: terminal normal white (`terminal.ansiWhite`) is now a muted gray, distinguishable from bright white in terminal output
- Removed raw HTML from the README so it renders correctly in the extension gallery
- Removed stale scopes from the generic constant rule (numbers and characters keep their dedicated colors)
- Excluded pnpm lock and workspace files from the published VSIX (smaller package)

### Changed
- Added palette colors (54 keys per theme) for surfaces that previously used VS Code defaults: command center, prominent/compact status bar items, status bar warning and error states, input validation, minimap scrollbar, diff editor lines and overview, peek view, editor line highlight and link active state, indent guides, dimmed line numbers, plus global error and icon foregrounds

## [0.2.3] - 2026-09-17

### Docs
- Added color swatches to the palette tables in the README
- Normalized relative image paths so gallery images render correctly
- Manual install section now links to the GitHub Releases page

## [0.2.2] - 2026-09-17

### Changed
- Migrated to pnpm as the project package manager
- First GitHub Release with a prebuilt VSIX asset

## [0.2.1] - 2026-09-17

### Fixed
- Added `.vscodeignore` so internal files (`.atl/` cache, `.gitignore`) are excluded from the published VSIX

## [0.2.0] - 2026-09-09

### Added
- Complete UI color coverage: sticky scroll, overview ruler, settings, quick input, welcome page, notifications, breadcrumbs, panels, peek view, symbol icons and merge editor
- `tab.activeBorderTop` indicator to clearly mark the active tab
- `input.foreground` / `input.placeholderForeground` for readable forms
- Semantic token colors now use standard VS Code token types
- Markdown inline code, strikethrough and bold headings
- Packaging scripts (`vsce`) and valid extension `name` for publishing

### Fixed
- Dark theme: `terminal.ansiBrightCyan` duplicated BrightBlue value
- Light theme: bright terminal colors inverted (e.g. BrightYellow darker than normal)
- `semanticTokenColors` used non-standard keys (`arithmetic`, `attribute`) that were ignored
- Conflicting `keyword.other` scopes between two token rules
- Barely-visible dark line numbers (`#27345C` -> `#3a4a75`)

## [0.1.0] - 2026-08-19

### Added
- Initial release
- Dark theme with semantic highlighting
- Light theme with semantic highlighting
- Custom color palette for both themes
- Support for VS Code and VSCodium

### Features
- Semantic token coloring for better code understanding
- Bracket pair colorization
- Git decorations support
- Terminal color support
