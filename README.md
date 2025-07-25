# Windows XAML Styles
A collection of my custom Windows XAML styles for Windhawk's various XAML styler mods for Windows 11.

## File Explorer

For [Windows 11 File Explorer Styler](https://windhawk.net/mods/windows-11-file-explorer-styler)

[JSON code](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/styles/FileExplorer.json)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/FileExplorer.png)

* Removed the tab's Close button - To close the tab, middle-click it or press `Ctrl`+`W`.
* Navigation Bar & Command Bar:
  * Alternative button glyphs: Back, Forward, Up, More
  * Mica effect extended to the Command Bar
  * Italicised search box text - The same way it was in Windows Vista and 7
* Details Pane:
  * Dynamic image container height
  * Removed the Share button
* Context Menu:
  * Removed the two "Share" menu items
  * Removed the "Show more options" menu item - To use the legacy context menu, hold Shift + right-click.
  * Removed the "Search the Microsoft Store" menu item from the "Open with" sub-menu -
    For other languages, replace `Search the Microsoft Store` in `MenuFlyoutItem[Text=Search the Microsoft Store]`.
  * Removed the keyboard accelerator text labels (such as: `Enter`, `Ctrl+Shift+C`, `Alt+Enter`, etc.) -
    Only the text labels are removed, without affecting the keyboard shortcuts' functionality.

## Notification Center

For [Windows 11 Notification Center Styler](https://windhawk.net/mods/windows-11-notification-center-styler)

[JSON code (for Dark theme)](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/styles/NotificationCenter-Dark.json)
| [JSON code (for Light theme)](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/styles/NotificationCenter-Light.json)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/MediaControls.png)

* Large album art image for the Quick Actions' Media Controls
* Translucent Text Input background - Read the "further configuration" section after first applying styles.

## Lock Screen

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) - Target process: `LockApp.exe`

[JSON code](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/styles/LockScreen.json)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/LockScreen.png)

* Moved the Time & Date HUD to the top-left corner of the screen
* Media Controls:
  * Large album art image
  * Translucent background
* Removed the UI elements for Fun Facts, Tips, and "Like the image that you see?",
those can be turned off via System Settings → Personalisation → Lock screen, but it affects only the non-Spotlight pics.
These custom styles can force remove them from Spotlight pics too.

## System Settings

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) - Target process: `SystemSettings.exe`

[JSON code](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/styles/SystemSettings.json)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/SystemSettings.png)

* Custom user pane text, replace the user name text and "Local Account" text (or email address text, if linked with a MS account) with anything you want -
  Read the "further configuration" section after first applying styles.
* Removed the MS 365 and OneDrive buttons from the System section
* Changed the pill shaped search box to a rectangle shaped one
* Made the network data usage indicator bars less eyesore with Dark theme
* Made the (Bluetooth) device names split into multi-lines instead of ellipsis

## How to apply Custom XAML Styles

First, install [Windhawk](https://windhawk.net/).

### File Explorer, Notification Center

1. Launch the Windhawk app.
2. Click the "Explore" button.
3. Find and install the "Windows 11 [process] Styler" mod.
4. Go to the mod's "Advanced" tab.
5. Clear everything in the "Mod settings" text box.
6. Copy the JSON code from this GitHub repo.
7. Paste the JSON code into the "Mod settings" text box.
8. Click "Save", and the changes take effect instantly.

### Lock Screen, System Settings

1. [Fork a Styler mod](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Forking-Styler-Mod-for-Other-UWP-Apps.md).
2. Find the forked Styler mod in the "Installed Mods" section.
3. Go to the mod's "Advanced" tab.
4. Clear everything in the "Mod settings" text box.
5. Copy the JSON code from this GitHub repo.
6. Paste the JSON code into the "Mod settings" text box.
7. Click "Save", and the changes take effect instantly.


## Further configuration

### Notification Center: Translucent Text Input Background

<details>
  <summary>
    Click to expand
  </summary>
  <ol>
    <li>
      Launch the Windhawk app.
    </li>
    <li>
      Find the "Windows 11 Notification Center Styler" mod.
    </li>
    <li>
      Go to the mod's "Advanced" tab.
    </li>
    <li>
      Add <code>TextInputHost.exe</code> to the custom process inclusion list.
    </li>
    <li>
      Click "Save".
    </li>
    <li>
      Go to System Settings → Personalisation → Text input, and use Dark theme.
    </li>
    <li>
      Restart <code>TextInputHost.exe</code> with Task Manager for changes to take effect.
    </li>
  </ol>
</details>

### System Settings: Custom User Pane Text

<details>
  <summary>
    Click to expand
  </summary>
  <ol>
    <li>
      Launch the Windhawk app.
    </li>
    <li>
      Find the forked Styler mod in the "Installed Mods" section.
    </li>
    <li>
      Go to the mod's "Settings" tab.
    </li>
    <li>
      Uncomment (remove <code>// </code> from) the first two targets: <code>TextBlock#UserName</code> and <code>TextBlock#UserAccount</code>.
    </li>
    <li>
      Edit the text in <code>Text=</code>.
    </li>
    <li>
      Click "Save settings".
    </li>
  </ol>
</details>


## How to make my own custom XAML styles?

Follow the [UWPSpy usage guide](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

Once you know how to customise the UWP apps and want to customise the Lock Screen too, check out the
[Lock Screen styling guide](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Lock-Screen-Styling-Guide.md).
