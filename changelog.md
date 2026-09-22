## Changelog

### 0.0.2.2
- Removed some orphaned code.

### 0.0.2.1
- Various documentation updates.
- Potential recipes for swapping are now checked to ensure that resources to produce them exist. If not, they are not considered for swaps.

### 0.0.2.0
- Moved from allowlist to blocklist. This change supports custom recipes in a better fashion.
- Added `RecipeSwapbackbuffers.txt`. This can be configured to set global or per recipe buffers for recipe swapback thresholds.
	- When swapping away from a recipe, the mod checks `currentStock >= productionLimit`.
	- The mod will attempt to prioritize swapping back to the original recipe, doing so when `currentStock <= (productionLimit - swapbackBuffer)`
	- Note that there is currently no mechanism for tracking the original recipe across play sessions.

### 0.0.1.1
- Expanded allowlist entries.

### 0.0.1.0
- Initial alpha release. 