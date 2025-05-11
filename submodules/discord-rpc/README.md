This fork modifies only one thing  
It adds support for custom buttons  
Discord Rich Presence can show max 2 buttons

More info:
- https://discord.com/developers/docs/events/gateway-events#activity-object-activity-structure
- https://discord.com/developers/docs/events/gateway-events#activity-object-activity-buttons

Usage example
```cpp
presence.buttonLabel[0] = "test1";
presence.buttonUrl[0] = "https://google.com";
presence.buttonLabel[1] = "test2";
presence.buttonUrl[1] = "https://youtube.com";
Discord_UpdatePresence(&presence);
```