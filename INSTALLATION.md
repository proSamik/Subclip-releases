# Subclip Installation Guide

## Download & Install

1. **Download**: Get the latest version from [GitHub Releases](https://github.com/proSamik/Subclip-releases/releases/latest)
2. **Install**: Double-click the DMG file and drag Subclip to Applications

## Fix "App is damaged" Error

If you see: **"Subclip" is damaged and can't be opened. You should move it to the Trash.**

**This is NOT actual corruption - it's just a macOS security warning.**

### Quick Fix (30 seconds)

1. **Open Terminal** (Press `Cmd + Space`, type "Terminal", press Enter)

2. **Copy and paste this command**:
   ```bash
   xattr -cr /Applications/Subclip.app
   ```

3. **Press Enter** and close Terminal

4. **Launch Subclip** - it will now open normally

### Alternative Methods

**Option 1: Right-Click Method**
- Right-click Subclip.app → **Open** → Click **Open** in the warning

**Option 2: System Settings** (if available)
- **System Settings** → **Privacy & Security** → Click **Open Anyway**

## Why This Happens

Subclip is an independent app not signed with Apple's $99/year certificate. The app is completely safe - this is just Apple's security warning for non-App Store apps.

## Troubleshooting

**If Terminal command doesn't work:**
- Make sure Subclip is in `/Applications/` folder
- Try: `xattr -cr ~/Desktop/Subclip.app` (if it's on Desktop)
- Or replace the path with wherever Subclip is located

**Still having issues?**
- [Report on GitHub Issues](https://github.com/proSamik/Subclip-releases/issues)
- Include your macOS version and exact error message

## System Requirements

- macOS 10.15 (Catalina) or later
- Apple Silicon (M1/M2/M3) and Intel Macs supported