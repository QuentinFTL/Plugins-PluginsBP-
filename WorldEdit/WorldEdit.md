# Object

# Properties

# Non-Static

- (string) wand: typeId of item used for positions selections. (default="minecraft:wooden_axe")
- (callback(playerBreakBlock)) itemUseOn: callback for first selection. (default=null)
- (callback(itemUseOn)) itemUseOn: callback for second selection. (default=null)


# Static

- (WorldEdit) instance: we use this property to get worldEdit instance from other file etc, and to only have 1 instance, to avoid multiple events.

# Installations
You must have theses plugins installed before this plugin in plugins.js:
- CorePlugin
- Permissions

# LOG

- 07/02/2024:
    -  WorldEdit (v0.0.2)
        -    Dependencies: (Permission, Core)
        -    Added Permissions Handler.
    -  Permission (v0.0.1)


- 06/02/2024:
    -  WorldEdit (v0.0.1)
        - base selection with the wooden axe (like the original plugin)
