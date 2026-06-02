# Windows XAML Styles
A collection of my custom Windows XAML styles for Windhawk's various XAML styler
mods for Windows 11.

These styles have been tested on Win11, version 25H2.

## Styles for Apps using XAML
* [File Explorer](#file-explorer)
* [Notification Center & Control Center](#notification-center--control-center)
* [Lock Screen](#lock-screen)
* [System Settings](#system-settings)
* [Windows Security](#windows-security)

## Info
* [How to apply Custom XAML Styles](#how-to-apply-custom-xaml-styles)
* [Further configuration](#further-configuration)
* [How to make my own custom XAML styles?](#how-to-make-my-own-custom-xaml-styles)

---

## File Explorer

For [Windows 11 File Explorer Styler](https://windhawk.net/mods/windows-11-file-explorer-styler)

[YAML code](/styles/FileExplorer.yaml)

![](/screenshots/FileExplorer.png)

### List of UI tweaks:
* Removed the tab's Close button
  * ℹ️ To close the tab, middle-click it or press `Ctrl`+`W`.
* Navigation Bar & Command Bar:
  * Alternative button glyphs: Back, Forward, Up, More
  * Mica effect extended to the Command Bar
  * Italicised search box text - The same way it was in Windows Vista and 7
* Details Pane:
  * Dynamic image container height
  * Removed the Share button
* Context Menu:
  * Removed the two "Share" menu items
  * Removed the "Show more options" menu item
    * ℹ️ To use the legacy context menu, hold Shift + right-click.
  * Removed the "Search the Microsoft Store" menu item from the "Open with"
    sub-menu
    * ℹ️ For other languages, replace `Search the Microsoft Store` in
      `MenuFlyoutItem[Text=Search the Microsoft Store]`.
  * Removed the keyboard accelerator text labels (such as: `Enter`,
    `Ctrl+Shift+C`, `Alt+Enter`, etc.)
    * ℹ️ Only the text labels are removed, without affecting the keyboard
      shortcuts' functionality :)

---

## Notification Center & Control Center

For [Windows 11 Notification Center Styler](https://windhawk.net/mods/windows-11-notification-center-styler)

[YAML code (for Dark theme)](/styles/NotificationCenter-Dark.yaml)
| [YAML code (for Light theme)](/styles/NotificationCenter-Light.yaml)

![](/screenshots/MediaControls.png)

![](/screenshots/NotificationCenter.png)

### List of UI tweaks:
* Notification Center:
  * Dynamic notifications container height
  * Compact "No new notifications" view
* Calendar:
  * Changed the circle shaped day/month/year slots to square shaped ones
  * Removed the focus assist section
* Control Center
  * Appears from the right (instead of bottom), just like the Notification
    Center
  * Large album art image for the Media Controls
* Translucent Text Input background
  * ℹ️ Read the "further configuration" section after first applying styles.

---

## Lock Screen

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) -
Target process: `LockApp.exe`

[YAML code](/styles/LockScreen.yaml)

![](/screenshots/LockScreen.png)

### List of UI tweaks:
* Moved the Time & Date HUD to the top-left corner of the screen
* Media Controls:
  * Translucent background
  * Large album art image
* Widgets:
  * Translucent background
  * Aligned to the bottom-left of screen instead of bottom-center
  * Custom title text - Replace the Weather location name with anything you
    want. No more leaking your current location! :D
    * ℹ️ Read the "further configuration" section after first applying styles.
* Removed the UI elements for Fun Facts, Tips, and "Like the image that you
  see?"
  * ℹ️ Those can be turned off via System Settings → Personalisation → Lock
    screen, but it affects only the non-Spotlight pics.
    These custom styles can force remove them from Spotlight pics too.

---

## System Settings

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) -
Target process: `SystemSettings.exe`

[YAML code](/styles/SystemSettings.yaml)

![](/screenshots/SystemSettings.png)

### List of UI tweaks:
* Custom user profile text - Replace the user name text and "Local Account" text
  (or email address text, if linked with a MS account) with anything you want.
  No more leaking your real/full name and email address! :D
  * ℹ️ Read the "further configuration" section after first applying styles.
* Removed the MS 365 and OneDrive buttons from the System page
* Changed the pill shaped search box to a rectangle shaped one
* Made the unfilled portion of network data usage indicator bars less eyesore
  with Dark theme

  <details>
    <summary>
      <b>
        Network data usage indicator bars: Before & After screenshots (click
        here to expand)
      </b>
    </summary>

    **Before:**
    ![](/screenshots/SystemSettings-NetworkDataUsageBars-Before.png)

    **After:**
    ![](/screenshots/SystemSettings-NetworkDataUsageBars-After.png)
  </details>

* Wrapped the (Bluetooth) device names into two lines

---

## Windows Security

For [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler) -
Target process: `SecHealthUI.exe`

[YAML code](/styles/WindowsSecurity.yaml)

![](/screenshots/WindowsSecurity.png)

### List of UI tweaks:
* Acrylic background
* Semi-bold page title font - The same way it is in Windows 11's System Settings

---

## How to apply Custom XAML Styles

First, install [Windhawk](https://windhawk.net/).

<details>
  <summary>
    <b>File Explorer / Notification Center & Control Center</b>
  </summary>

  1. Launch the Windhawk app.
  2. Click the "Explore" button.
  3. Find and install the "Windows 11 [process] Styler" mod.
  4. Go to the mod's "Settings" tab.
  5. Switch to "Textual mode" and clear everything in the text editor.
  6. Copy the YAML code from this GitHub repo.
  7. Paste the YAML code into the mod settings' text editor.
  8. Click "Save settings", and the changes take effect instantly.
</details>

<details>
  <summary>
    <b>Lock Screen / System Settings / Windows Security</b>
  </summary>

  1. [Fork a Styler mod](/guides/Forking-Styler-Mod-for-Other-UWP-Apps.md),
     changing a target process to:
     * `LockApp.exe` for Lock Screen
     * `SystemSettings.exe` for System Settings
     * `SecHealthUI.exe` for Windows Security
  2. Find the forked Styler mod in the "Installed Mods" section.
  3. Go to the mod's "Settings" tab.
  4. Switch to "Textual mode" and clear everything in the text editor.
  5. Copy the YAML code from this GitHub repo.
  6. Paste the YAML code into the mod settings' text editor.
  7. Click "Save settings", and the changes take effect instantly. If the System
     Settings or Windows Security app is open, close and relaunch it.
</details>


## Further configuration

<details>
  <summary>
    <b>Translucent Text Input Background</b>
  </summary>

  1. Launch the Windhawk app.
  2. Find the "Windows 11 Notification Center Styler" mod.
  3. Go to the mod's "Advanced" tab.
  4. Add `TextInputHost.exe` to the custom process inclusion list.
  5. Click "Save".
  6. Go to System Settings → Personalisation → Text input, and use Dark theme.
  7. Restart `TextInputHost.exe` with Task Manager for changes to take effect.
</details>

<details>
  <summary>
    <b>Lock Screen: Custom Widgets Title Text</b>
  </summary>

  1. Launch the Windhawk app.
  2. Find the forked Styler mod in the "Installed Mods" section.
  3. Go to the mod's "Settings" tab.
  4. Add this target to the Target text box:
     `StackPanel#WidgetGroupPanel > ContentPresenter[1] > LockCanvas.LockCanvasWidgetFrame > Grid > Grid#WidgetFrameGrid > Grid > ContentControl#WidgetHeaderContent > ContentPresenter > Widgets.UWP.WidgetView.WidgetHeader > Grid > StackPanel#DefaultTitleStackPanel > TextBlock`
     * The number [1] in `ContentPresenter[1]` corresponds to Widgets' 1st slot.
       To change the Weather widget's title (location name) in the 2nd/3rd/4th
       slot, change [1] to [2], [3], or [4].
  5. Add `Text=` to the Styles text box, and type anything after it - example:
     `Text=Windhawk Streets`.
  6. Click "Save settings", and the changes take effect instantly.
</details>

<details>
  <summary>
    <b>System Settings: Custom User Profile Text</b>
  </summary>

  1. Launch the Windhawk app.
  2. Find the forked Styler mod in the "Installed Mods" section.
  3. Go to the mod's "Settings" tab.
  4. Uncomment (remove `// ` from) the first two targets: `TextBlock#UserName`
     and `TextBlock#UserAccount`.
  5. Edit the text in `Text=`.
  6. Click "Save settings", and the changes take effect the next time you launch
     the Settings app.
</details>


## How to make my own custom XAML styles?

Follow the [UWPSpy usage guide](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

Once you know how to customise the UWP apps and want to customise the Lock
Screen too, check out the
[Lock Screen styling guide](/guides/Lock-Screen-Styling-Guide.md).
