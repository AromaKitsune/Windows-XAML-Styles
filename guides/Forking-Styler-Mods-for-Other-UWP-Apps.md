# Forking Mods for Other UWP Apps
This section shows how to fork the styler mods for other UWP apps such as Lock Screen.

- Install [Windhawk](https://windhawk.net/)
- Launch the Windhawk app
- Explore the mods
- Search and pick a "Windows 11 Start Menu Styler" mod
- Click "Details", then "Install"
- After install, click the "Fork" button

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork1.png)

- On the editor, change the ID and name of the mod
- Remove the two lines of target processes, and replace the remaining target process with a different one: LockApp.exe for Lock Screen

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork2.png)

![](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/screenshots/Fork3.png)

- When done, click the "Compile Mod" button

- Now you can copy the JSON code from this GitHub repo and paste it into the forked mod settings → Advanced tab → "Mod settings" text box
