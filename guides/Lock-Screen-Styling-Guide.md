# Lock Screen Styling Guide
This section shows how to customise the Lock Screen for Windows 10 and Windows 11.

If this is your first time customising the XAML styles, check out the UWPSpy guide [here](https://github.com/bbmaster123/FWFU/blob/main/uwpspy.md).

1. Launch UWPSpy as administrator
2. Look for `LockApp.exe`. If it doesn't show up, lock your PC at least once by pressing `Win`+`L`, unlock your PC, then click "Refresh"
3. While `LockApp.exe` is selected, press `Tab` twice so it selects the "Spy" button
4. Press `Enter` then immediately `Win`+`L`
5. The UWPSpy window should appear on the Lock Screen, you can now customise it

[Video in action](https://drive.google.com/file/d/196NVuEpOtcZAGzzDaRucDCyfrcdYlghp/view?usp=sharing)

While customising the Lock Screen, you cannot copy the target names to clipboard. To workaround this:
1. Resize the UWPSpy window so it shows the tree-view of target names you want to copy
2. Take a screenshot by pressing `Win`+`PrtScr`, or just `PrtScr`
3. Unlock your PC
4. Launch MS Paint
5. Paste the screenshot by pressing `Ctrl`+`V`
6. Take a screenshot of the UWPSpy window's tree-view with `Shift`+`Win`+`S`
7. Click the Snipping Tool notification to launch Snipping Tool
8. Use the text extraction (OCR) feature and copy all texts
9. Paste the texts into Notepad. Since the OCR is not perfect, make sure to correct the spellings of target names

Once you got those target names, add them to a [forked Styler mod](https://github.com/AromaKitsune/Windows-XAML-Styles/blob/main/guides/Forking-Styler-Mod-for-Other-UWP-Apps.md).

## Clock & Date HUD

### Clock & Date HUD container

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

### Clock HUD

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
HorizontalAlignment=Lef
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
Grid#Networklcon
```

### Battery indicator icon

Target:
```
Image#BatteryStatusProvider
```

