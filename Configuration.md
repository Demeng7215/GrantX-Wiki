# Configuration
Configuring GrantX to your liking.

## Configuration Files
A list of configuration files with their factory default values can be found in [this folder](https://github.com/Demeng7215/GrantX-Wiki/tree/master/configs). Files ending in **.db** are NOT configuration files and you should not touch them if you don't know what you are doing unless you want to corrupt grant data.

## Available Materials
Since GrantX focuses on GUI menus, there are many cases in the config files where you need to enter a material name. [Click here](https://github.com/Demeng7215/GrantX-Wiki/blob/master/Available%20Materials.java) for a list of valid materials.

## Placeholders
A list of placeholders you can use in configuration files. Some placeholders may return the word "not applicable", depending on the situation (eg. %revoke-time% will return N/A if the grant has not been revoked yet).

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
| %issuer-uuid% | The UUID of the issuer. |
| %revoker% | The username of the grant revoker player. |
| %revoker-uuid% | The UUID of the revoker. |
| %revoke-time% | The time of when the grant was revoked. |
| %expiration% | The time of which the grant will expire (or the word "never"). |
| %rank-{placeholder} | Use any rank placeholder by adding the **rank-** prefix to the placeholder. |
| %server-{placeholder} | Use any server placeholder by adding the **server-** prefix to the placeholder. |
| %duration-{placeholder} | Use any duration placeholder by adding the **duration-** prefix to the placeholder. |
| %reason-{placeholder} | Use any reason placeholder by adding the **reason-** prefix to the placeholder. |

### Rank Placeholders 
| Placeholder | Description |
|-------------|----------------------------------------------------------------|
| %id% | The unique identifier of the rank. |
| %type% | The type of rank- Rank or Permission. |
| %real-name% | The real name (group/node) of the rank. |
| %weight% | The weight of the rank. |
| %slot% | The slot of the rank. |
| %material% | The name of the material representing the rank. |
| %display-name% | The display name of the rank. |
| %stripped-display-name% | The display name of the rank, without color. |
| %lore-type% | The type of lore- Default, Custom, None.
| %permission% | The permission required to choose the rank. |
| %dummy% | If this rank is a dummy- Yes or No. |
| %grantable% | If this rank is grantable. Exact opposite of dummy. |
| %glow% | If this rank will glow in GUIs- Yes or No. |
| %blacklisted-servers% | The servers where this rank cannot be chosen. |
| %blacklisted-servers-count% | The number of servers where this rank cannot be chosen. |
