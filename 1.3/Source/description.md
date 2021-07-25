Allows building floors out of stuff*.

# Important
You can safely add this mod to you save games, but *you can not remove it* from save games. (If you really must do this, you'll have to remove all built stuffed floors added by this mod first).

# Features
This mod does two things. First, using Architect Sense it provides a framework for modders to define their own stuffed floor types. Second, it uses this framework to create a number of new floors that are stuffed. 

**For players**
Adds several floor types (borrowed with permission from Telkir's [More Floors](http://steamcommunity.com/sharedfiles/filedetails/?id=725623521), CuproPanda's [Extra Floors](https://ludeon.com/forums/index.php?topic=13400#msg135940) and Pravus' [Fences and Floors](http://steamcommunity.com/sharedfiles/filedetails/?id=784370602)) in a variety of stone, wood and metal types.

Works great with other mods that add more resources, e.g. [Minerals and Materials](http://steamcommunity.com/sharedfiles/filedetails/?id=728233992) [Kura's Extra Minerals](http://steamcommunity.com/sharedfiles/filedetails/?id=852103845), [Extended Woodworking](http://steamcommunity.com/sharedfiles/filedetails/?id=836912371), [Vegetable Garden](http://steamcommunity.com/sharedfiles/filedetails/?id=822470192) and [GlitterTech](http://steamcommunity.com/sharedfiles/filedetails/?id=725576127). 

This mod also organizes and where needed, removes the floors added by Vanilla RimWorld, [More Floors](http://steamcommunity.com/sharedfiles/filedetails/?id=725623521), [Extended Woodworking](http://steamcommunity.com/sharedfiles/filedetails/?id=836912371), [Minerals and Materials](http://steamcommunity.com/sharedfiles/filedetails/?id=728233992), [GlitterTech](http://steamcommunity.com/sharedfiles/filedetails/?id=725576127), [More Furniture](http://steamcommunity.com/sharedfiles/filedetails/?id=739089840), [Vegetable Garden](http://steamcommunity.com/sharedfiles/filedetails/?id=822470192) and [Floored](http://steamcommunity.com/sharedfiles/filedetails/?id=801544922).

**For modders**
Adds a custom FloorTypeDef that derives from TerrainDef, and allows modders to create floortypes by setting a texture (grayscale for best effect, will be coloured by stuff) and a list of stuffCategories to generate terrain defs for. The resulting designators will be placed together in a category, and any vanilla or other mod's terrains made obsolete can also be provided in the XML, and will then be hidden for the user (but not removed, so it won't break save games).

# Known issues
While this mod will happily generate more floors for any mods that add materials to the metallic, stony and/or woody stuff types, it only cleans up the floors added by mods that are explicitly supported. Any other mods that add floor types may appear as duplicates. If you encounter such an issue, please let the author(s) of said mod(s) know so that they can correctly set up their designator groups! 

# Technical details
*: This mod doesn't actually allow building stuffed floors. Rather, it spoofs this behaviour by generating TerrainDefs for each of the stuffDefs handed to it, and then adds them to 'DesignatorDropdownGroups' to group these terrains together and give a user experience similar to stuff selection on buildings. The way it does this is exactly the same as the vanilla tile floors (which was stolen from an earlier version of this mod), but for more floors, and all available stuff types. This mod doesn't do anything destructive, it doesn't make any detours, and doesn't remove any defs. It does however remove a number of designators from the architect in order to hide them from the user.

# Powered by Harmony
![Powered by Harmony](https://camo.githubusercontent.com/074bf079275fa90809f51b74e9dd0deccc70328f/68747470733a2f2f7332342e706f7374696d672e6f72672f3538626c31727a33392f6c6f676f2e706e67)
