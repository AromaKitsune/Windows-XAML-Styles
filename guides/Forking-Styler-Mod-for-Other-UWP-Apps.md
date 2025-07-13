# Forking Styler Mod for Other UWP Apps
This section shows how to fork a Styler mod for other UWP apps such as Lock Screen.

> [!NOTE]
> Custom lock screen styles do not preserve after log out or system restart since Windhawk mods are loaded into RAM.

1. Launch the Windhawk app.
2. Explore the mods.
3. Search and pick a "Windows 11 Start Menu Styler" mod.
4. Click "Details", then "Install".
5. After install, click the "Fork" button.

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork1.png)

6. On the editor, change an ID and name of a mod.
7. Remove the two lines of target processes, and replace the remaining target process with a different one:
  - `LockApp.exe` for Lock Screen
  - `SystemSettings.exe` for System Settings

Before:
![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork2.png)

After:
![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork3.png)

8. When done, click the "Compile Mod" button.
9. Click "Exit Editing Mode".
10. Find the forked Styler mod.
11. Click "Details".
12. Go to the "Advanced" tab.
13. Clear everything in the "Mod settings" text box.
14. Go to this GitHub repo.
15. Open the JSON file for a specific process.
16. Copy the whole code.
17. Go back to the Windhawk app.
18. Paste the JSON code into the "Mod settings" text box.
19. Click "Save", and the changes take effect instantly.
