# Materials
Materials are the things that this mod revolves around. Each material can be as unique or as similar as one desires, the only thing that needs to be unique is its full [`ResourceLocation`](https://minecraft.wiki/w/Resource_location) (i.e. `kubejs:iridium` and `foobar:iridium` - this would be considered unique due to the namespace being different, but i don't recommend it, since you start falling into the problem of 3+ mods adding the exact same thing with absolutely no use of oredict/item tags to allow for interchangeability).

Material definitions are (currently) split into three inner classes within [`Material.java`](https://github.com/The-Incipisphere/Perfectly-Ungeneric-Objects/blob/main/src/main/java/io/thedogofchaos/perfectlyungenericobjects/common/material/Material.java) in `io.thedogofchaos.perfectlyungenericobjects.common.material`
## Info
> Inner class name: **`MaterialInfo`**

This inner class stores key information about a material, such as its ID (in `ResourceLocation` format), an `IntList` of colours, its assigned texture set, and whether or not additional colours have already been assigned to the aforementioned `IntList`.
## Components
> Inner enum name: **`MaterialComponents`**

A component is basically a representation of a physical form that a material can take.
Each material can have whatever combination of components that one desires, and the mod will generate items/blocks/fluids accordingly.
### List of current Components
- **`INGOT`**: https://en.wikipedia.org/wiki/Ingot - (Mutually exclusive with **`GEM`**)
- **`NUGGET`**:
- **`STORAGE_BLOCK`**:
- **`DUST`**:
- **`GEM`**: (Mutually exclusive with **`INGOT`**)
## Flags
> Inner class name: **`MaterialFlags`**

allan please add details about flags
### List of current Flags
- **`HAS_COMPRESSION_RECIPES`**