Here's the `.md` file for `Dialog_Show` as requested:

---

title: Dialog_Show
description: Shows a dialog to a player using the specified parameters.
tags: ["dialog", "easyDialog"]

---

## Description

Displays a dialog to a player with the given parameters such as dialog style, caption, info, and buttons.

| Parameter     | Description                                                                                 |
|---------------|---------------------------------------------------------------------------------------------|
| playerid      | The ID of the player to show the dialog to.                                                 |
| dialog        | The dialog identifier (name) to be used.                                                    |
| style         | The style of the dialog (e.g., DIALOG_STYLE_MSGBOX, DIALOG_STYLE_INPUT, DIALOG_STYLE_LIST). |
| caption[]     | The title or caption of the dialog.                                                         |
| info[]        | The content or information to be displayed in the dialog.                                   |
| button1[]     | The text for the first button.                                                              |
| button2[]     | The text for the second button (optional).                                                  |
| {Float,_}:... | Variadic parameters to accommodate additional float parameters.                             |

## Examples

```pawn
CMD:weapons(playerid, params[]) {
    Dialog_Show(playerid, WeaponMenu, DIALOG_STYLE_LIST, "Weapon Menu", "9mm\nSilenced 9mm\nDesert Eagle\nShotgun\nSawn-off Shotgun\nCombat Shotgun", "Select", "Cancel");
    return 1;
}

Dialog:WeaponMenu(playerid, response, listitem, inputtext[]) {
    if (response) {
        new str[64];
        format(str, 64, "You have selected the '%s'.", inputtext);

        GivePlayerWeapon(playerid, listitem + 22, 500);
        SendClientMessage(playerid, -1, str);
    }
    return 1;
}

public OnDialogPerformed(playerid, const dialog[], response, success) {
    if (!strcmp(dialog, "WeaponMenu") && IsPlayerInAnyVehicle(playerid)) {
        SendClientMessage(playerid, -1, "You must be on-foot to spawn a weapon.");
        return 0;
    }
    return 1;
}
```

## Notes

:::tip

This function is part of the `easyDialog` include, which makes dialog management simpler by using named dialogs instead of IDs.

:::

## Related Functions

- [Dialog_Close](Dialog_Close): Closes any opened dialogs for the specified player.
- [Dialog_Opened](Dialog_Opened): Checks if a dialog is opened for the specified player.

---

Let me know if there's anything else you need or if you have any adjustments in mind! 😊
