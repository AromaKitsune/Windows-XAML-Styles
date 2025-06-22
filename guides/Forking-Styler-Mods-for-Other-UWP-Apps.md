# Forking Styler Mods for Other UWP Apps
This section shows how to fork the Styler mods for other UWP apps such as Lock Screen.

1. Launch the Windhawk app
2. Explore the mods
3. Search and pick a "Windows 11 Start Menu Styler" mod
4. Click "Details", then "Install"
5. After install, click the "Fork" button

  ![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork1.png)

7. On the editor, change the ID and name of the mod
8. Remove the two lines of target processes, and replace the remaining target process with a different one: `LockApp.exe` for Lock Screen

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork2.png)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork3.png)

9. When done, click the "Compile Mod" button

10. Now you can copy the JSON code from this GitHub repo and paste it into the forked mod settings → Advanced tab → "Mod settings" text box
