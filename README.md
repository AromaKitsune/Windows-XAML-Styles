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

## Notification Center

For [Windows 11 Notification Center Styler](https://windhawk.net/mods/windows-11-notification-center-styler)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/MediaControls.png)

* Large album art image for the Quick Actions' Media Controls

## Lock Screen

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) - See the mods forking guide on the bottom of the page.

Target process: `LockApp.exe`

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/LockScreen.png)

* Moved the Clock & Date HUD to the top-left corner of the screen
* Removed the UI elements for Fun facts, tips & "Like the image that you see?",
those can be turned off via Settings → Personalisation → Lock screen, but it affects only the non-Spotlight pics.
These custom styles can force remove them for Spotlight pics too.
* Large album art image for the Media Controls

## How to apply Custom XAML Styles

1. Install [Windhawk](https://windhawk.net/)
2. Launch the Windhawk app
3. Explore the mods
4. Search and pick a Styler mod you want to install
5. Click "Details", then "Install"
6. Go to the "Advanced" tab
7. Clear everything in the "Mod settings" text box
8. Go to this GitHub repo
9. Open the JSON file for a specific Styler mod
10. Copy the whole code
11. Go back to the Windhawk app
12. Paste the JSON code into the "Mod settings" text box
13. Click "Save", and the changes take effect instantly

## How to make my own custom XAML styles?

Check out the UWPSpy guide [here](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

For other UWP apps such as Lock screen, check out the [forking Styler mods guide](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Forking-Styler-Mods-for-Other-UWP-Apps.md)
and [Lock Screen styling guide](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Lock-Screen-Styling-Guide.md).
