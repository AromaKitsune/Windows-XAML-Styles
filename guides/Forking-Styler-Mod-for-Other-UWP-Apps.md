# Forking Styler Mod for Other UWP Apps
This section shows how to fork a Styler mod to target other UWP processes such as Lock Screen.

> [!NOTE]
> Custom lock screen styles do not preserve after log out or system restart since Windhawk mods are loaded into RAM.

1. Launch the Windhawk app.
2. Click the "Explore" button.
3. Find and install the "Windows 11 Start Menu Styler" mod.
4. After install, click the "Fork" button.

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork1.png)

5. On the editor, change an ID and name of a mod.
6. Remove the two lines of target processes, and replace the remaining target process with a different one:
  - `LockApp.exe` for Lock Screen
  - `SystemSettings.exe` for System Settings
  - `SecHealthUI.exe` for Windows Security

Before:
![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork2.png)

After:
![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork3.png)

7. When done, click the "Compile Mod" button.
8. Click "Exit Editing Mode", and this compiled mod should appear in the "Installed Mods" section.
