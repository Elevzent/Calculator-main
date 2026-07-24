# Changelog
## 2026-07-25

### Added

- Added the default gold 1x3 item named `三个-横条`.

### Changed

- Kept the item-library and inventory table headers visible while their lists scroll.
- Replaced the fixed four-Worker cap with a device-aware limit, capped at 12 while preserving capacity for page interaction.

## 2026-07-21

### Added

- Added fast and deep solver modes.
- Added optional 2-4 Worker parallel search with global best-result merging.
- Added synchronized optional-column controls for the item library and inventory.
- Added responsive mobile item cards and collapsible screenshot recognition.
- Added a live inventory cell summary showing used cells, available cells, and the remaining or excess count.

### Changed

- Cached repeated singleton completion states and streamed improved solver results to the UI.
- Reworked desktop table columns to fill their containers based on visible-column weights.
- Gave the inventory bonus-description column additional width for readable text.
- Allowed vertical page scrolling to begin anywhere inside mobile item cards.
- Centered the empty-inventory message across the full table width.
- Changed default item qualities to purple for single-cell items, gold for 2-4-cell items, and red for 5-cell items.

### Fixed

- Fixed hidden columns reserving blank table space.
- Fixed optional numeric columns expanding beyond their content.
- Fixed hidden controls remaining visible because of generic label styles.
- Fixed mobile table controls overflowing or intercepting vertical page scrolling.
