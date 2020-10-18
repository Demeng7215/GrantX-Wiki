# Configuration
Configuring GrantX to your liking.

## Configuration Files
A list of configuration files with their factory default values can be found in [this folder](https://github.com/Demeng7215/GrantX-Wiki/tree/master/configs). Files ending in **.db** are NOT configuration files and you should not touch them if you don't know what you are doing unless you want to corrupt grant data.

## Available Materials
Since GrantX focuses on GUI menus, there are many cases in the config files where you need to enter a material name. [Click here](https://github.com/Demeng7215/GrantX-Wiki/blob/master/Available%20Materials.java) for a list of valid materials.

## Placeholders
A list of placeholders you can use in configuration files.

### Grant Placeholders
| Placeholder | Description |
|-------------|----------------------------------------------------------------|
| %id% | The unique identifier of the grant. |
| %status% | The current status of the grant (Active, Expired, or Revoked). |
| %time% | The formatted date and time of when the grant was activated. |
| %date% | The formatted date (no time) of when the grant was activated. |
| %target% | The username of the grant target player. |
| %target-uuid% | The UUID of the target. |
| %issuer% | The username of the grant issuer player (or the word "console"). |
| %issuer-uuid% | The UUID of the issuer (or the word "not applicable"). |
| %revoker% | The username of the grant revoker player (or the word "not applicable"). |
| %revoker-uuid% | The UUID of the revoker (or the word "not applicable"). |
