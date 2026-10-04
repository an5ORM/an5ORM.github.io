# Changelog

## [Unreleased]

### Changed
- The favicon is generated from the `an5Brand` tokens instead of a hand-copied SVG
  that drew the wordmark as live text, so the browser tab no longer depends on which
  fonts the machine has.
- Brand colours come from the generated token block instead of 21 hardcoded hex and
  `rgba()` literals. `--cyan` and `--blue` now resolve to `--an5-gradient-start` and
  `--an5-gradient-end`, and the wordmark badge uses `--an5-gradient`.
- `npm test` also runs `brand:check`, which fails if the favicon or the brand token
  block drift from `an5Brand/tokens.json`.

### Fixed
- `--border-hover` was `rgba(99,179,237,0.3)`, which is not the brand indigo. It is
  now the brand indigo at the same alpha.

### Added
- The VS Code extension is announced on both registries: the VS Code Marketplace is the
  primary card and install button, Open VSX stays available for VSCodium and other
  VS Code-compatible editors, and the footer links both.
- `robots.txt` and `sitemap.xml` with production URLs.
- JSON-LD (`WebSite`, `SoftwareSourceCode`), `canonical`, Open Graph and Twitter card
  metadata.

### Changed
- The landing page says "Go" rather than "Golang".

## [0.0.1] - 2026-08-19

- chore: update misc

## [0.1.0] - 2026-08-19

- Add `an5example` package card (multi-dialect CRUD suite, browser support, TS/Go/.NET/Python examples)
- Add `an5example` to footer Packages links

