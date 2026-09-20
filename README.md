# whiskerwood-productionlimitsloader
A mod that adds a widget to save and load production limits.

## Overview
 - Production Limits Loading
 	- Pressing `/` will save the current production limits to disk. 
 	- Pressing `ctrl+/` it will reload the last save. 
 	- Primarily useful for quickly applying a default set of production limits to a new colony.
 - Automatic Recipe Swaps
 	- Industries that are set to produce something that is over the production limit will attempt to swap to a new recipe every 10 seconds.
 	- Add recipes to `RecipeWhitelist.txt` to enable them for selection. Only whitelisted recipes are considered. 

