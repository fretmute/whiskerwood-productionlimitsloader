## Changelog

### 0.0.2.0
- Moved from whitelist to blacklist. This change supports custom recipes in a better fashion.
- Added `RecipeSwapbackbuffers.txt`. This can be configured to set global or per recipe buffers for recipe swapback thresholds.
	- When swapping away from a recipe, the mod checks `currentStock >= productionLimit`.
	- The mod will attempt to prioritize swapping back to the original recipe, doing so when `currentStock <= (productionLimit - swapbackBUffer)`
	- Note that there is currently no mechanism for tracking the original recipe across play sessions.

### 0.0.1.1
- Expanded whitelist entries.

### 0.0.1.0
- Initial alpha release. 