# Commands and Permissions
List of commands and permissions.

## Commands
### /grantx
**Description:** Base command, displays plugin information.

### /grantx help
**Description:** Displays a list of commands.

### /grantx editor
**Description:** Opens the in-game rank, server, duration, and reason editor.
**Permission:** grantx.editor

### /grantx logs [issuer]
**Description:** Opens the grant logs menu. Specifying a player will only show grants issued by that specific player. Otherwise, all issued grants will be shown. </br>
**Permission:** grantx.logs

### /grantx delete <id>
**Description:** Permanently deletes the grant with the specified ID from the database.</br>
**Permission:** grantx.delete

### /grantx import
**Description:** Import ranks from your permissions plugin into GrantX.</br>
**Permission:** grantx.import

### /grantx addProtection <player>
**Description:** Prevent other people from granting the specified player and viewing their previous grants.</br>
**Permission:** grantx.addprotection

### /grantx removeProtection <player>
**Description:** Remove protection from the specified player.</br>
**Permission:** grantx.removeprotection

### /grantx updateCache
**Description:** Forcibly update the local player cache on the current server.</br>
**Permission:** grantx.updatecache

### /grantx reload
**Description:** Reloads all configuration files.</br>
**Permission:** grantx.reload

### /grant [player] [rank] [server] [duration] [reason]
**Description:** Issue a new grant. If no player argument is provided, player selector will open. If the player name is the only argument, the normal grant GUI will open. If rank, server, duration, and reason are all provided, there will be no GUI or confirmation and the grant will be forcibly activated.</br>
**Permission:** grantx.grant

### /grants [player]
**Description:** View the specified player's grant history. If no player is specified, player selector will open first.</br>
**Permission:** grantx.grants

## Standalone Permissions
These permissions are not directly related to any commands.

### grantx.bypassprotection
**Description:** Bypass any protection a player may have.

## grantx.revoke.<rank>
**Description:** Permission to revoke ranks with the specified ID in grant history menus.
