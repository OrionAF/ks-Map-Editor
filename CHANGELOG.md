# Changelog

All notable changes to this project will be documented in this file.

## [0.3.1.2] - Patch

### Changed
- Re-made the mobile layout.  This is just a test.

## [0.3.1.1] - Minor

### Changed
- **Bookmarks can now be multi-pinned!** Instead of a single pinned favorite, you can now pin an unlimited number of landmarks.
- Pinned bookmarks are now displayed as a persistent list in the top-right corner for immediate access. Each item has its own 'Go' and 'Unpin' buttons.
- The expandable bookmark menu is now solely for adding new pins from a list of available (unpinned) landmarks.

## [0.3.1.0] - Major

### Added
- **New Advanced Bookmarks System!**
  - Replaced the basic dropdown with a new expandable bookmark menu located conveniently under the minimap.
  - **Pin a Favorite:** You can now pin a landmark! The pinned location is displayed when the menu is closed and is remembered across sessions.
  - Each bookmark now has its own "Go" button for one-click navigation.

### Changed
- **Major UI Layout Overhaul:**
  - The performance stats (FPS, Tiles) have been moved to a permanently visible panel in the top-left corner.
  - The `Settings` button and panel have been relocated to the bottom-right corner. The panel now expands upwards.
  - The version number display has been moved to the bottom-left corner for a cleaner layout.
- The bookmark menu now smoothly slides up to fill the space when the minimap is hidden.
- Adjusted the height of the vertical zoom slider for better compatibility with various screen aspect ratios.
- On smaller screens (under 768px wide), only the minimap is hidden, keeping the new bookmark and settings panels accessible.

### Removed
- The previous bookmark dropdown from within the `Settings` panel.
- The `Stats` button (📊), as the performance stats are now always visible.

## [0.3.0.0] - Major

### Added
- **New Feature: Bookmarks!** 
A new dropdown menu has been added to the Settings panel, allowing you to instantly jump to any Fortress, Sanctuary or the King's Castle.
- Added new `+10%` and `-10%` buttons to the zoom controls for faster, larger zoom adjustments.

### Changed
- The "Go To" and "Bookmark" navigation functions now zoom to a standard 100% level, providing a more consistent experience.
- The layout of the left-side zoom controls has been adjusted to accommodate the new buttons.
- The "Presets" dropdown now resets to a placeholder after a selection is made, allowing you to select a value, zoom in/out, and select the same value again.

## [0.2.9.2] - Patch

### Fixed
- **Tile selecting:** Fixed the single tile selecting feature which broke in the last major update.  Before this update, it only worked for building tiles.  This has now been fixed.


## [0.2.9.1] - Minor

### Changed
- Refactored the patch notes system to load and render directly from this `CHANGELOG.md` file.
- This simplifies the update process and ensures a single source of truth for all changes.

### Removed
- The `patch_notes.json` file is no longer used by the application and has been deprecated.

## [0.2.9.0] - Major

### Changed
- The minimap has been completely rebuilt to render as a true isometric representation of the main map, instead of a simple 2D grid.
- The minimap now intelligently zooms and pans to stay focused on your viewport, providing better contextual awareness when zoomed in, while remaining static at low zoom.
- The zoom slider has been moved further to the left of the screen and made longer to make it easier to use.
- The coordinate search box has been moved to the bottom center of the screen.
- UI elements now dynamically resize and reposition based on the available space to support various screen sizes and devices.
  - The minimap is now hidden on displays with a width less than 768px.
  - The tool detects if the screen is in landscape or portrait mode and adjusts the layout accordingly.

### Added
- **New Zoom Presets:** Replaced the zoom preset buttons with a more compact dropdown menu and added a wider range of presets: 5%, 10%, 15%, 20%, 40%, 60%, and 80%.
- **More Tile-Merging Presets:** Added new tile-merging presets for 20%, 40%, 50%, 60%, 70% and 80% zoom levels for more granular performance control.

### Fixed
- **Predictable Zooming:** Corrected the behavior of the `+` / `–` zoom buttons. They now increment/decrement the zoom by exactly 1% instead of a variable amount, providing more precise control.

## [0.2.8.0] - Patch

### Changed
- Updated viewport camera icon.
- Other minor tweaks.

## [0.2.7.7] - Patch

### Changed
- The minimap viewport indicator is now drawn as a diamond, accurately reflecting the main map's isometric camera view.
- The fill and border colors of the minimap viewport indicator have been adjusted for better contrast against biome colors.
- The minimap toggle button has been made slimmer with reduced padding and a slightly smaller font for a less obtrusive look.
- Minimap canvas internal padding has been significantly reduced, minimizing the visible 'border' effect from the background color.

## [0.2.7.6] - Minor

### Added
- The minimap can now be shown or hidden using a new integrated toggle button.

### Changed
- The minimap has been significantly enlarged for better visibility and detail.
- The toggle button is styled as a sleek bar at the top of the minimap, effectively replacing the previous thick padding border for a cleaner look.

## [0.2.7.5] - Patch

### Changed
- Made some improvements to the minimap.

## [0.2.7.4] - Minor

### Added
- Implemented **Markdown** support for displaying patch notes using the `marked.js` library.

### Changed
- Notes can now include *italics*, **bold text**, lists, and other Markdown features for improved readability.

## [0.2.7.3] - Minor

### Changed
- The minimap now dynamically zooms relative to the main map's zoom level.
- The minimap's view now centers on the main map's current viewport.
- Adjusted the 'Fit' zoom level to ensure better map visibility on load.
- Improved minimap scale calculation and added further guards against invalid numeric states.

### Fixed
- Resolved an issue where the Settings panel would overlap the minimap when opened.
- Corrected main map drawing functions to resolve a black screen issue.

## [0.2.7.0] - Major

### Added
- A new minimap is now available in the top-right corner, providing an overview of the entire game world.
- Display toggles, Performance settings, and Info/Stats are now consolidated into a new collapsible '⚙️ Settings' panel in the top-right.

### Changed
- Key structures (King's Castle, Fortresses) and Biome regions are now displayed on the minimap.
- The 'Go To' coordinate search has been moved to the top of the left-side panel.
- Updated the Stats button icon to 📊.
- Clicking on the minimap will now instantly pan the main map to that location.

### Fixed
- Corrected a minor HTML class name typo in the patch notes modal footer.

## [0.2.6.3] - Patch

### Changed
- Made some minor performance improvements.

## [0.2.6.2] - Patch

### Changed
- Made a few tweaks to adjust zooming feel and responsiveness.

## [0.2.6.1] - Patch

### Fixed
- Attempted to fix an issue with the statistics panel not updating correctly.

## [0.2.6.0] - Major

### Added
- Added a 'ping' effect: selections now flash briefly to make them easier to locate on the map.

### Changed
- Completed a major internal code refactor for improved long-term stability and easier future updates.
- The settings panel in the top-right has been reorganized with headers for better clarity.

### Fixed
- Fixed a minor performance issue where buildings were being drawn twice.

## [0.2.5.12] - Minor

### Added
- Added a new 'Always Show RSS' toggle for Alliance RSS buildings. When enabled, this will keep Alliance RSS buildings visible on the map at all zoom levels.

### Fixed
- Fixed a rendering bug that was causing buildings to be drawn twice in high-detail view.

## [0.2.5.11] - Patch

### Changed
- Refactored the building rendering logic to be more efficient.

### Fixed
- Fixed a critical bug where Alliance RSS buildings were not filling their entire 2x2 area, leaving parts of the tile uncolored.

## [0.2.5.10] - Patch

### Fixed
- Fixed a bug where Alliance RSS buildings were rendered as 1x1 tiles instead of the correct 2x2 size.
- Fixed an issue where the names of Alliance RSS buildings (e.g., 'Wood', 'Food') were not being displayed on the map.

## [0.2.5.9] - Minor

### Added
- A new toggleable layer for 'Alliance RSS' buildings.
- Alliance resource nodes (Wood, Food, Stone, Iron) will now render on the map with unique colors.
- A new 'Show Alliance RSS' checkbox has been added to control their visibility.

## [0.2.5.8] - Minor

### Added
- New 'Tile Detail' setting now controls only when tiles merge together at low zoom levels.
- New 'Show Gridlines' checkbox gives users direct control over gridline visibility.

### Changed
- Replaced the confusing 'Quality' dropdown with two separate, clearer settings.

## [0.2.5.7] - Minor

### Added
- Added a 'Quality' dropdown menu in the top-right panel.

### Changed
- Users can now choose their preferred performance vs. visual quality setting.
- The selected quality setting is saved and remembered for your next visit.

## [0.2.5.5] - Patch

### Changed
- Made improvements to the zoom camera behavior.

## [0.2.5.4] - Minor

### Changed
- Changed the color palette of existing buildings.
- Implemented Sanctuaries on the map.

## [0.2.5.3] - Patch

### Fixed
- Fixed the patch notes not showing and updating correctly.

## [0.2.5.2] - Minor

### Changed
- Improved the vertical zoom slider for better precision and a more consistent layout on different screen sizes.
- Optimized application startup by moving patch notes to an external file.

## [0.2.5.1] - Major

### Added
- Added a vertical zoom slider on the left.
- Added this patch notes window and versioning system.

### Changed
- Redesigned UI layout for improved usability.
- Implemented a configurable display for tile coordinates.

### Fixed
- Fixed building name text overflowing its container.

## [0.2.5.0] - Initial Release

### Added
- Initial public release version with core features.