# Object

# - Properties
- Non-Static
    - (string) wand: typeId of item used for positions selections. (default="minecraft:wooden_axe")
    - (callback(playerBreakBlock)) itemUseOn: callback for first selection. (default=null)
    - (callback(itemUseOn)) itemUseOn: callback for second selection. (default=null)

- Static
    - (WorldEdit) instance: we use this property to get worldEdit instance from other file etc, and to only have 1 instance, to avoid multiple events.

# Methods
  
- Non-Static
    - (void) toggleOffWand(sender): remove the ability to select with wand tool for sender.
        - sender: Player | Entity

    - (void) toggleOnWand(sender): add the ability to select with wand tool for sender.
        - sender: Player | Entity
  
    - (void) set(sender, pattern): fill the selection area with block(pattern).
        - sender: Player | Entity
        - pattern: string

    - (number) distance(a, b): return the distance between 2 numbers (a and b).
        - a: number
        - b: number

    - (bool) sameLocation(a, b): return true if location of a is equal to location of b.
        - a: Vector3
        - b: Vector3

- Static
    - (void) wand(sender): give the wand tool to sender if he has the needed permissions.
        - sender: Player | Entity

    - (void) toggleeditwand(sender): toggle the ability to select with wand tool for sender.
        - sender: Player | Entity
        

# Installations
You must have theses plugins installed before this plugin in plugins.js:
- CorePlugin

# LOG

- 07/02/2024:
    -  Permission (v0.0.1)
        -    Dependencies: (Core)
        -    Added Permissions Manager (js file containing json object).
