Here's a `.md` file similar to the one you provided, for the miscellaneous natives:

---

title: Streamer_Miscellaneous_Natives
description: Provides miscellaneous native functions for the streamer.
tags: ["native-functions", "miscellaneous"]

---

## Description

Provides miscellaneous native functions for the streamer.

| Name                         | Description                                                                                                              |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Streamer_GetDistanceToItem   | Gets the distance to an item from specified coordinates.                                                                  |
| Streamer_ToggleItem          | Toggles the visibility of an item for a player.                                                                           |
| Streamer_IsToggleItem        | Checks if an item is toggled for a player.                                                                                |
| Streamer_ToggleAllItems      | Toggles the visibility of all items for a player, with optional exceptions.                                               |
| Streamer_GetItemInternalID   | Gets the internal ID of an item for a player.                                                                             |
| Streamer_GetItemStreamerID   | Gets the streamer ID of an item for a player.                                                                             |
| Streamer_IsItemVisible       | Checks if an item is visible to a player.                                                                                 |
| Streamer_DestroyAllVisibleItems | Destroys all visible items for a player, optionally serverwide.                                                      |
| Streamer_CountVisibleItems   | Counts the number of visible items for a player, optionally serverwide.                                                   |
| Streamer_DestroyAllItems     | Destroys all items of a specified type, optionally serverwide.                                                            |
| Streamer_CountItems          | Counts the number of items of a specified type, optionally serverwide.                                                    |
| Streamer_GetNearbyItems      | Gets nearby items of a specified type within a range from specified coordinates.                                           |
| Streamer_GetAllVisibleItems  | Gets all visible items for a player.                                                                                      |
| Streamer_GetItemPos          | Gets the position of an item.                                                                                             |
| Streamer_SetItemPos          | Sets the position of an item.                                                                                             |
| Streamer_GetItemOffset       | Gets the offset of an item.                                                                                               |
| Streamer_SetItemOffset       | Sets the offset of an item.                                                                                               |

## Examples

```c
public OnGameModeInit()
{
    Float:distance;
    Streamer_GetDistanceToItem(2000.0, 1500.0, 10.0, 1, 1001, distance); // Example usage of Streamer_GetDistanceToItem.
    Streamer_ToggleItem(0, 1, 1001, 1); // Example usage of Streamer_ToggleItem.
    return 1;
}
```

## Notes

:::tip

These miscellaneous native functions can help manage and manipulate items in various ways, enhancing the gameplay experience.

:::

## Related Functions

- [Streamer_GetDistanceToItem](Streamer_GetDistanceToItem): Gets the distance to an item.
- [Streamer_ToggleItem](Streamer_ToggleItem): Toggles an item for a player.
- [Streamer_IsToggleItem](Streamer_IsToggleItem): Checks if an item is toggled for a player.
- [Streamer_ToggleAllItems](Streamer_ToggleAllItems): Toggles all items for a player.
- [Streamer_GetItemInternalID](Streamer_GetItemInternalID): Gets the internal ID of an item.
- [Streamer_GetItemStreamerID](Streamer_GetItemStreamerID): Gets the streamer ID of an item.
- [Streamer_IsItemVisible](Streamer_IsItemVisible): Checks if an item is visible.
- [Streamer_DestroyAllVisibleItems](Streamer_DestroyAllVisibleItems): Destroys all visible items for a player.
- [Streamer_CountVisibleItems](Streamer_CountVisibleItems): Counts visible items for a player.
- [Streamer_DestroyAllItems](Streamer_DestroyAllItems): Destroys all items of a specified type.
- [Streamer_CountItems](Streamer_CountItems): Counts the number of items of a specified type.
- [Streamer_GetNearbyItems](Streamer_GetNearbyItems): Gets nearby items within a specified range.
- [Streamer_GetAllVisibleItems](Streamer_GetAllVisibleItems): Gets all visible items for a player.
- [Streamer_GetItemPos](Streamer_GetItemPos): Gets the position of an item.
- [Streamer_SetItemPos](Streamer_SetItemPos): Sets the position of an item.
- [Streamer_GetItemOffset](Streamer_GetItemOffset): Gets the offset of an item.
- [Streamer_SetItemOffset](Streamer_SetItemOffset): Sets the offset of an item.

---

Let me know if this suits your needs or if there's anything else you'd like to add! 😊
