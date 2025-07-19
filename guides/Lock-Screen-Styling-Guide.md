# Lock Screen Styling Guide
This section shows how to customise the Lock Screen for Windows 10 and Windows 11.

If this is your first time customising the XAML styles, check out the [UWPSpy usage guide](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

> [!NOTE]
> Custom lock screen styles do not preserve after log out or system restart since Windhawk mods are loaded into RAM.

1. Launch UWPSpy.
2. Look for `LockApp.exe`. If it doesn't show up, lock your PC at least once by pressing `Win`+`L`, unlock your PC, then click "Refresh".
3. Select `LockApp.exe`.
4. Press `Enter` then immediately `Win`+`L`.
5. The UWPSpy window should appear on the Lock Screen, you can now customise it.

https://github.com/user-attachments/assets/0d58605e-544b-4918-99bf-126fc54bafec

While customising the Lock Screen, you cannot copy the target elements texts to clipboard. To workaround this:
1. Resize the UWPSpy window so it shows the tree-view of target elements you want to copy.
2. Take a screenshot by pressing `Win`+`PrtScr`, or just `PrtScr`.
3. Unlock your PC.
4. Launch MS Paint.
5. Paste the screenshot by pressing `Ctrl`+`V`.
6. Take a screenshot of the UWPSpy window's tree-view with `Win`+`Shift`+`S`.
7. Click the Snipping Tool notification to launch Snipping Tool.
8. Use the text extraction (OCR) feature and copy all texts.
9. Paste the texts into Notepad. Since the OCR is not perfect, make sure to manually correct the spellings of target elements.

Once you got those target elements:
1. [Fork a Styler mod](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Forking-Styler-Mod-for-Other-UWP-Apps.md).
2. Find the forked Styler mod in the "Installed Mods" section.
3. Click "Details".
4. Go to the "Settings" tab.
5. Add those targets and styles in the "Control styles" section.
6. Click "Save", and the changes take effect instantly.


## Time & Date HUD

### Time & Date HUD container

Target:
```
StackPanel#TimeAndDatePanel
```

Styles:
```
VerticalAlignment=Top
HorizontalAlignment=Left
Margin=50,20,0,0
```

### Time HUD

Target:
```
StackPanel#TimePanel > TextBlock#Time
```

Style:
```
HorizontalAlignment=Left
```

### Date HUD

Target:
```
StackPanel#TimeAndDatePanel > TextBlock#Date
```

Style:
```
HorizontalAlignment=Left
```

## Bottom-right icons

### Bottom-right icons container

Target:
```
StackPanel#StatusProviderPanel
```

### Network icon

Target:
```
Grid#NetworkIcon
```

### Battery indicator icon

Target:
```
Image#BatteryStatusProvider
```
