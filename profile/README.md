# ADB AppControl - Disable or Remove Android Packages from the PC

## At a Glance

Phones hide some packages behind a friendly name and keep others as system apps you cannot uninstall in Settings. ADB AppControl asks adb for the package list and shows it in a table. Disable is the reversible test. Uninstall for the user is stronger. A full uninstall of a system package can return after an update or can break a feature if you picked the wrong name.

- USB debugging already enabled by the owner
- An authorization tap on the phone
- Package names visible before any change
- Disable first, uninstall only when you know the name
- A saved list so you can undo a preset

The phone is yours or you are sitting with the person who can unlock it. A tool that removes apps is not a way into a phone that is locked.

## Disable versus Remove

| Action | What remains | Use it when |
|---|---|---|
| Disable | The package stays, it does not run | You are testing a bloat app |
| Uninstall for user | Hidden for this user, often restorable | You do not want it in the drawer |
| Uninstall system app | May be gone until a firmware restore | You have the package name from a note, not a guess |
| Reinstall or enable | The undo | Something you use broke |
| A downloaded preset | Someone else's phone | Do not apply it blindly |

System UI, permission controllers, and the package installer are not clutter. If the name is vague, leave it. A lighter home screen is not worth a phone that cannot show a dialog.

## Session

1. Enable USB debugging and accept the PC fingerprint on the phone.
2. Connect and load the package list.
3. Search for one app you can see on the phone and match its package name.
4. Disable that one entry.
5. Unplug, use the phone, and confirm the feature you care about still exists.
6. Only then disable a second app, or undo the first from the same list.

Save your own preset after it has survived a day. A preset from the internet names packages that may not exist on your build, or may exist and matter.

Large OEM skins rename nothing important in a way you can trust from the label alone. The package name is the column that counts. Sort by system or user if the tool offers it, and stay inside user apps until you have a written reason to touch a system package. Disabling a dozen system packages in one afternoon produces a phone that boots to a broken launcher, and the undo is the preset you did not save.

![ADB AppControl package list with one app disabled](https://www.smartzone.de/wp-content/uploads/2022/06/bloatware-auf-android-einfach-entfernen-mit-adb-appcontrol-anleitung/adb-appcontrol-website.png)

## Who It Fits

Owners cleaning preinstalled apps on a phone they can unlock. A poor fit for a locked phone, a stolen phone, or a wish to remove device-admin protections you did not put there. A poor fit for a full firmware change. Packages are not partitions.

[![Open ADB AppControl](https://img.shields.io/badge/Open-ADB_AppControl-1f6feb?style=for-the-badge&logo=android&logoColor=white)](https://cavaleridosal44.github.io/.github/adb-appcontrol-debloat)

## Requirements

| Item | Expectation |
|---|---|
| Phone | Unlocked, with USB debugging on |
| PC | Windows, a working adb driver |
| Cable | Data |
| Undo | The enable or install button, plus a preset you saved |
| Patience | One package at a time on the first day |

## Fixes

The list is empty. The phone did not authorize the PC, or debugging is off.
An app returns after reboot. It is a system package that the vendor restores, or you only disabled a shortcut.
The launcher crashed. Re-enable the last packages you touched before you disable more.
USB disconnects during a batch. Stop the batch. Finish or undo what already changed, one name at a time.
You applied a preset and the dialer vanished. Restore the preset's disabled entries. Do not factory-reset as the first undo.

## Keep a Note

Write down the package names you disabled, not the icons. After a system update, open the list again. Vendors put apps back, and they sometimes add new ones. Your old preset is a starting point only if those names still exist. If the phone misbehaves, the note is the undo list. Memory of "a few Samsung apps" is not.

## Names, Not Icons

ADB AppControl is safe in proportion to how slowly you use it. Disable one package whose name you matched to an icon you can see. Use the phone. Then decide. A preset from the internet is a list of someone else's build.

- USB debugging on, and the allow tap done
- One user app first
- System UI and the package installer left alone
- Preset saved only after a day
- Enable is the undo
- System update may restore apps
- Launcher crash means undo before more disables
- Cable is data, or the list stays empty
- Locked phone is out of scope
- Firmware flash is a different tool

| Action | Risk |
|---|---|
| View the list | None |
| Disable a named user app | Low if you can enable it |
| Uninstall a system package | High without a note |
| Apply a downloaded preset | High |
| Batch while the cable drops | Unknown state |

Write the package names down. "A few vendor apps" is not an undo list.

## Reference Lines

adb appcontrol, adb appcontrol debloat, disable android apps pc, adb appcontrol windows, android package name list, disable not uninstall system app, adb appcontrol preset, usb debugging app list
