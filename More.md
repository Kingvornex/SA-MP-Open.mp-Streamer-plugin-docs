Here's a `.md` file for the natives related to pickups, checkpoints, race checkpoints, and map icons:

---

title: Streamer_Natives_Pickups_Checkpoints_Map_Icons
description: Provides native functions for pickups, checkpoints, race checkpoints, and map icons in the streamer.
tags: ["native-functions", "pickups", "checkpoints", "race-checkpoints", "map-icons"]

---

## Description

Provides native functions for pickups, checkpoints, race checkpoints, and map icons in the streamer.

| Name                           | Description                                                                                                               |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------- |
| CreateDynamicPickup            | Creates a dynamic pickup at specified coordinates.                                                                         |
| DestroyDynamicPickup           | Destroys a dynamic pickup.                                                                                                |
| IsValidDynamicPickup           | Checks if a dynamic pickup is valid.                                                                                       |
| CreateDynamicCP                | Creates a dynamic checkpoint at specified coordinates.                                                                     |
| DestroyDynamicCP               | Destroys a dynamic checkpoint.                                                                                            |
| IsValidDynamicCP               | Checks if a dynamic checkpoint is valid.                                                                                   |
| IsPlayerInDynamicCP            | Checks if a player is in a dynamic checkpoint.                                                                             |
| GetPlayerVisibleDynamicCP      | Gets the visible dynamic checkpoint for a player.                                                                          |
| CreateDynamicRaceCP            | Creates a dynamic race checkpoint at specified coordinates.                                                               |
| DestroyDynamicRaceCP           | Destroys a dynamic race checkpoint.                                                                                       |
| IsValidDynamicRaceCP           | Checks if a dynamic race checkpoint is valid.                                                                              |
| IsPlayerInDynamicRaceCP        | Checks if a player is in a dynamic race checkpoint.                                                                        |
| GetPlayerVisibleDynamicRaceCP  | Gets the visible dynamic race checkpoint for a player.                                                                     |
| CreateDynamicMapIcon           | Creates a dynamic map icon at specified coordinates.                                                                       |
| DestroyDynamicMapIcon          | Destroys a dynamic map icon.                                                                                              |
| IsValidDynamicMapIcon          | Checks if a dynamic map icon is valid.                                                                                      |

## Examples

```c
public OnGameModeInit()
{
    // Example usage of CreateDynamicPickup
    CreateDynamicPickup(1274, 2, 2000.0, 1500.0, 10.0);
    
    // Example usage of CreateDynamicCP
    CreateDynamicCP(2000.0, 1500.0, 10.0, 5.0);
    
    // Example usage of CreateDynamicRaceCP
    CreateDynamicRaceCP(1, 2000.0, 1500.0, 10.0, 2005.0, 1505.0, 10.0, 5.0);
    
    // Example usage of CreateDynamicMapIcon
    CreateDynamicMapIcon(2000.0, 1500.0, 10.0, 1, 0xFF0000FF);
    
    return 1;
}
```

## Notes

:::tip

These native functions can be used to create and manage pickups, checkpoints, race checkpoints, and map icons in your game, adding interactivity and enhancing the gameplay experience.

:::

## Related Functions

- [CreateDynamicPickup](CreateDynamicPickup): Creates a dynamic pickup.
- [DestroyDynamicPickup](DestroyDynamicPickup): Destroys a dynamic pickup.
- [IsValidDynamicPickup](IsValidDynamicPickup): Checks if a dynamic pickup is valid.
- [CreateDynamicCP](CreateDynamicCP): Creates a dynamic checkpoint.
- [DestroyDynamicCP](DestroyDynamicCP): Destroys a dynamic checkpoint.
- [IsValidDynamicCP](IsValidDynamicCP): Checks if a dynamic checkpoint is valid.
- [IsPlayerInDynamicCP](IsPlayerInDynamicCP): Checks if a player is in a dynamic checkpoint.
- [GetPlayerVisibleDynamicCP](GetPlayerVisibleDynamicCP): Gets the visible dynamic checkpoint for a player.
- [CreateDynamicRaceCP](CreateDynamicRaceCP): Creates a dynamic race checkpoint.
- [DestroyDynamicRaceCP](DestroyDynamicRaceCP): Destroys a dynamic race checkpoint.
- [IsValidDynamicRaceCP](IsValidDynamicRaceCP): Checks if a dynamic race checkpoint is valid.
- [IsPlayerInDynamicRaceCP](IsPlayerInDynamicRaceCP): Checks if a player is in a dynamic race checkpoint.
- [GetPlayerVisibleDynamicRaceCP](GetPlayerVisibleDynamicRaceCP): Gets the visible dynamic race checkpoint for a player.
- [CreateDynamicMapIcon](CreateDynamicMapIcon): Creates a dynamic map icon.
- [DestroyDynamicMapIcon](DestroyDynamicMapIcon): Destroys a dynamic map icon.
- [IsValidDynamicMapIcon](IsValidDynamicMapIcon): Checks if a dynamic map icon is valid.

---

Let me know if this covers everything or if there's anything else you'd like to tweak! 😊
