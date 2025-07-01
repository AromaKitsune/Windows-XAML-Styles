# Windows XAML Styles
A collection of my custom Windows XAML styles for Windhawk's various XAML styler mods for Windows 11.

## File Explorer

For [Windows 11 File Explorer Styler](https://windhawk.net/mods/windows-11-file-explorer-styler)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/FileExplorer.png)

* Custom button glyphs: Back, Forward, Up, More
* Mica effect extended to the Command Bar
* Dynamic image container height for the Details Pane
* Removed the tab's Close button (to close the tab, middle-click it or press `Ctrl`+`W`)
* Context Menu: Removed the Share options & "Show more options"
* Context Menu: Removed the "Search the Microsoft Store" menu item from the "Open with" sub-menu

## Notification Center

For [Windows 11 Notification Center Styler](https://windhawk.net/mods/windows-11-notification-center-styler)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/MediaControls.png)

* Large album art image for the Quick Actions' Media Controls
* Translucent Text Input - Read the "additional configuration" section after first applying styles

## Lock Screen

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) - Target process: `LockApp.exe`

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/LockScreen.png)

* Moved the Clock & Date HUD to the top-left corner of the screen
* Removed the UI elements for Fun facts, tips & "Like the image that you see?",
those can be turned off via System Settings → Personalisation → Lock screen, but it affects only the non-Spotlight pics.
These custom styles can force remove them for Spotlight pics too.
* Large album art image for the Media Controls

## System Settings

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) - Target process: `SystemSettings.exe`

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/SystemSettings.png)

* Replace the user name text with anything you want
* Replace the "Local Account" text or email address text (if linked with a MS account) with anything you want
* Removed the MS 365 and OneDrive buttons from the System page

## How to apply Custom XAML Styles

First, install [Windhawk](https://windhawk.net/).

### File Explorer, Notification Center

1. Launch the Windhawk app
2. Explore the mods
3. Search and pick a Styler mod for a specific process
4. Click "Details", then "Install"
5. Go to the "Advanced" tab
6. Clear everything in the "Mod settings" text box
7. Go to this GitHub repo
8. Open the JSON file for a specific Styler mod
9. Copy the whole code
10. Go back to the Windhawk app
11. Paste the JSON code into the "Mod settings" text box
12. Click "Save", and the changes take effect instantly

### Lock Screen, System Settings

Follow the [forking Styler mod guide](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Forking-Styler-Mod-for-Other-UWP-Apps.md).


## Additional configuration

### Translucent Text Input

1. Launch the Windhawk app
2. Find the "Windows 11 Notification Center Styler" mod
3. Click "Details"
4. Go to the "Advanced" tab
5. Add `TextInputHost.exe` to the custom process inclusion list
6. Click "Save"
7. Go to System Settings → Personalisation → Text input, and use Dark theme
8. Restart `TextInputHost.exe` with Task Manager for changes to take effect


## How to make my own custom XAML styles?

Follow the [UWPSpy usage guide](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

Once you know how to customise the UWP apps and want to customise the Lock Screen too, check out the
[Lock Screen styling guide](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Lock-Screen-Styling-Guide.md).
