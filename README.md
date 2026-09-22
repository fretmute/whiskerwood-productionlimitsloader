# whiskerwood-productionlimitsloader
A mod that adds various quality of life features around production limits.

## Overview
 - Production Limits Loading
 	- Pressing `/` will save the current production limits to disk. 
 	- Pressing `ctrl+/` it will reload the last save. 
 	- Primarily useful for quickly applying a default set of production limits to a new colony.
 - Automatic Recipe Swaps
 	- Industries that are set to produce something that is over the production limit will attempt to swap to a new recipe every 10 seconds.
 	- Recipes that do not have sufficient resources for production are not considered.
 	- Add recipes to `RecipeBlocklist.txt` to prevent their selection. Blocklisted recipes are never considered for swaps.
 	- `RecipeSwapbackbuffers.txt`
 		- This can be configured to set global or per recipe buffers for recipe swapback thresholds.
		- When swapping away from a recipe, the mod checks `currentStock >= productionLimit`.
		- The mod will attempt to prioritize swapping back to the original recipe, doing so when `currentStock <= (productionLimit - swapbackBuffer)`
		- Note that there is currently no mechanism for tracking the orignal recipe across play sessions.

