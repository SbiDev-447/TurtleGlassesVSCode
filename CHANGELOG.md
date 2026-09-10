# Changelog

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
