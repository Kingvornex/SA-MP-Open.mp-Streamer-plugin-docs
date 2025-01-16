create dynamic object.md
Here's a `.md` file that follows the structure you provided:

---

title: CreateDynamicObject
description: Creates a dynamic object at specified coordinates in the game world.
tags: ["dynamic-object"]

---

## Description

Creates a dynamic object at specified coordinates in the game world.

| Name               | Description                                                                                                               |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------- |
| modelid            | The model to create.                                                                                                      |
| Float:x            | The X coordinate to create the object at.                                                                                 |
| Float:y            | The Y coordinate to create the object at.                                                                                 |
| Float:z            | The Z coordinate to create the object at.                                                                                 |
| Float:rotationX    | The X rotation of the object.                                                                                             |
| Float:rotationY    | The Y rotation of the object.                                                                                             |
| Float:rotationZ    | The Z rotation of the object.                                                                                             |
| worldid            | (optional) The world ID to place the object in.                                                                            |
| interiorid         | (optional) The interior ID to place the object in.                                                                         |
| playerid           | (optional) The player ID to assign the object to.                                                                          |
| Float:streamdistance | (optional) The distance that the object is rendered from the player.                                                     |
| Float:drawdistance | (optional) The distance that objects are rendered at. 0.0 will cause objects to render at their default distances.         |
| areaid             | (optional) The area ID to place the object in.                                                                             |
| priority           | (optional) The priority of the object.                                                                                     |

## Examples

```c
public OnGameModeInit()
{
    CreateDynamicObject(2587, 2001.195679, 1547.113892, 14.283400, 0.0, 0.0, 96.0); // Object will render at its default distance.
    CreateDynamicObject(2587, 2001.195679, 1547.113892, 14.283400, 0.0, 0.0, 96.0, 300.0); // Object will render at 300.0 units.
    return 1;
}
```

## Notes

:::tip

There is a limit of 1000 objects (MAX_OBJECTS). To circumvent this limit, you can use the [streamer](https://github.com/samp-incognito/samp-streamer-plugin) plugin.

:::

## Related Functions

- [DestroyDynamicObject](DestroyDynamicObject): Destroy a dynamic object.
- [IsValidDynamicObject](IsValidDynamicObject): Checks if a certain dynamic object is valid.
- [MoveDynamicObject](MoveDynamicObject): Move a dynamic object.
- [StopDynamicObject](StopDynamicObject): Stop a dynamic object from moving.
- [SetDynamicObjectPos](SetDynamicObjectPos): Set the position of a dynamic object.
- [SetDynamicObjectRot](SetDynamicObjectRot): Set the rotation of a dynamic object.
- [GetDynamicObjectPos](GetDynamicObjectPos): Locate a dynamic object.
- [GetDynamicObjectRot](GetDynamicObjectRot): Check the rotation of a dynamic object.
- [AttachDynamicObjectToPlayer](AttachDynamicObjectToPlayer): Attach a dynamic object to a player.
- [SetDynamicObjectMaterialText](SetDynamicObjectMaterialText): Replace the texture of a dynamic object with text.
- [SetDynamicObjectMaterial](SetDynamicObjectMaterial): Replace the texture of a dynamic object with the texture from another model in the game.

---

Let me know if this works for you or if there’s anything else you need! 😊
