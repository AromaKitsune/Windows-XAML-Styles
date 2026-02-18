# Windows XAML Styles
A collection of my custom Windows XAML styles for Windhawk's various XAML styler
mods for Windows 11.

These styles have been tested on Win11, version 25H2.

## Table of contents
* Styles for UWP Apps
  * [File Explorer](#file-explorer)
  * [Notification Center & Control Center](#notification-center--control-center)
  * [Lock Screen](#lock-screen)
  * [System Settings](#system-settings)
  * [Windows Security](#windows-security)
* Info
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
    Before:
    <img src="/screenshots/SystemSettings-NetworkDataUsageBars-Before.png">
    After:
    <img src="/screenshots/SystemSettings-NetworkDataUsageBars-After.png">
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
  <ol>
    <li>
      Launch the Windhawk app.
    </li>
    <li>
      Click the "Explore" button.
    </li>
    <li>
      Find and install the "Windows 11 [process] Styler" mod.
    </li>
    <li>
      Go to the mod's "Settings" tab.
    </li>
    <li>
      Switch to "Textual mode" and clear everything in the text editor.
    </li>
    <li>
      Copy the YAML code from this GitHub repo.
    </li>
    <li>
      Paste the YAML code into the mod settings' text editor.
    </li>
    <li>
      Click "Save settings", and the changes take effect instantly.
    </li>
  </ol>
</details>

<details>
  <summary>
    <b>Lock Screen / System Settings / Windows Security</b>
  </summary>
  <ol>
    <li>
      <a href="/guides/Forking-Styler-Mod-for-Other-UWP-Apps.md">
      Fork a Styler mod</a>, changing a target process to:
      <ul>
        <li>
          <code>LockApp.exe</code> for Lock Screen
        </li>
        <li>
          <code>SystemSettings.exe</code> for System Settings
        </li>
        <li>
          <code>SecHealthUI.exe</code> for Windows Security
        </li>
      </ul>
    </li>
    <li>
      Find the forked Styler mod in the "Installed Mods" section.
    </li>
    <li>
      Go to the mod's "Settings" tab.
    </li>
    <li>
      Switch to "Textual mode" and clear everything in the text editor.
    </li>
    <li>
      Copy the YAML code from this GitHub repo.
    </li>
    <li>
      Paste the YAML code into the mod settings' text editor.
    </li>
    <li>
      Click "Save settings", and the changes take effect instantly. If the
      System Settings or Windows Security app is open, close and relaunch it.
    </li>
  </ol>
</details>


## Further configuration

<details>
  <summary>
    <b>Translucent Text Input Background</b>
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
      Restart <code>TextInputHost.exe</code> with Task Manager for changes to
      take effect.
    </li>
  </ol>
</details>

<details>
  <summary>
    <b>Lock Screen: Custom Widgets Title Text</b>
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
      Add <code>StackPanel#WidgetGroupPanel > ContentPresenter[1] >
      LockCanvas.LockCanvasWidgetFrame > Grid > Grid#WidgetFrameGrid > Grid >
      ContentControl#WidgetHeaderContent > ContentPresenter >
      Widgets.UWP.WidgetView.WidgetHeader > Grid >
      StackPanel#DefaultTitleStackPanel > TextBlock</code> to the Target text
      box.
      <ul>
        <li>
          The number [1] in <code>ContentPresenter[1]</code> corresponds to
          Widgets' 1st slot. To change the Weather widget's title (location
          name) in the 2nd/3rd/4th slot, change [1] to [2], [3], or [4].
        </li>
      </ul>
    </li>
    <li>
      Add <code>Text=</code> to the Styles text box, and type anything after
      it - example: <code>Text=Windhawk Streets</code>.
    </li>
    <li>
      Click "Save settings", and the changes take effect instantly.
    </li>
  </ol>
</details>

<details>
  <summary>
    <b>System Settings: Custom User Profile Text</b>
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
      Uncomment (remove <code>// </code> from) the first two targets:
      <code>TextBlock#UserName</code> and <code>TextBlock#UserAccount</code>.
    </li>
    <li>
      Edit the text in <code>Text=</code>.
    </li>
    <li>
      Click "Save settings", and the changes take effect the next time you
      launch the Settings app.
    </li>
  </ol>
</details>


## How to make my own custom XAML styles?

Follow the [UWPSpy usage guide](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

Once you know how to customise the UWP apps and want to customise the Lock
Screen too, check out the
[Lock Screen styling guide](/guides/Lock-Screen-Styling-Guide.md).
