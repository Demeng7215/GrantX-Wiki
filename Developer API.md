# Developer API
GrantX comes with a developer API with several events, allowing developers to code their own custom addons to GrantX.

## Setting Up
### Using the API for a Public Project
Go to https://github.com/Demeng7215/GrantX-API and import the latest release (or the release you want) into your IDE or build configuration.

### Using the API for a Private Project
Simply import the actual plugin (GrantX's JAR) into your IDE or build configuration.

## Notes
* You cannot shade the API or compile it into your own JAR. The API is already provided in the actual plugin.
* Request more API methods at https://feedback.demeng.dev/.

## Usage
### Events
There are currently 3 events in the API:
* [dev.demeng.grantx.api.event.GrantActivateEvent](https://github.com/Demeng7215/GrantX-API/blob/master/src/main/java/dev/demeng/grantx/api/event/GrantActivateEvent.java) - Called after a grant is confirmed.
* [dev.demeng.grantx.api.event.GrantExpireEvent](https://github.com/Demeng7215/GrantX-API/blob/master/src/main/java/dev/demeng/grantx/api/event/GrantExpireEvent.java) - Called after a grant expires.
* [dev.demeng.grantx.api.event.GrantRevokeEvent](https://github.com/Demeng7215/GrantX-API/blob/master/src/main/java/dev/demeng/grantx/api/event/GrantRevokeEvent.java) - Called after a grant revocation is confirmed.<br>

You can use these as you would with vanilla Bukkit events, as such:
```java
public class MyAddonEvent implements Listener {
  @EventHandler
  public void onGrantActivate(GrantActivateEvent e) {
    // Code here
  }
}
```
As with normal events, you need to register the event in your onEnable method.
```java
Bukkit.getPluginManager().registerListeners(new MyAddonEvent(), this);
```

Each of these events are called with a [dev.demeng.grantx.api.Grant](https://github.com/Demeng7215/GrantX-API/blob/master/src/main/java/dev/demeng/grantx/api/Grant.java) object, which contains information about the grant that has been activated, expired, or revoked. Access this object by using #getGrant(). Methods in this class are documented ([click here](https://github.com/Demeng7215/GrantX-API/blob/master/src/main/java/dev/demeng/grantx/api/Grant.java)).
