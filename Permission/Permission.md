# Object

# - Properties
- Non-Static

- Static
    - ([Object]) grades: we use this property to get grades registered in Permission/permissions.js.

# Methods
  
- Non-Static

  
- Static
    - (void) give(sender, name, perm): give the permission (perm) to the player(name) by sender, if he has the rights to add the role (see Permission/permissions.js).
        - sender: Player | Entity
        - name: string
        - perm: string
    - (bool) canGivePermission(sender, perm = null): check if sender can give Permission(perm) by is rights or isOp().
        - sender: Player | Entity
        - perm: string | null
    - (undefined|string) get(player): get the permission of the player.
        - player: Player | Entity | string
    - <Warning>(void) set(player, perm): set the permission(perm) to player (Warning: this can set every permissions, without permission, so don't allow people to access this method with any command without conditions !)
          - player: Player | Entity | string
          - perm: string
        - (bool) includes(perm): Check if permission(perm) is registered in Permission/permissions.js.
          - perm: string
        - (void) unset(player): remove all permissions of player.
            - player: Player | Entity | string
        - (bool) static has(player, permission = ""): if permission = "", check if player as any permission, else, it check if the player has the target(s) permission(s).
            - player: Player | Entity | string
            - permission: string | string[] 
        

# Installations
You must have theses plugins installed before this plugin in plugins.js:
- CorePlugin

# LOG

- 07/02/2024:
    -  Permission (v0.0.1)
        -    Dependencies: (Core)
        -    Added Permissions Manager (js file containing json object).
