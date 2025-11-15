# Mac PDF Viewer Crashes - Preview and Adobe Fix Guide

# Mac PDF Viewer Crashes - Preview and Adobe Fix Guide

**PDF viewer crashing on macOS?** This guide fixes crashes in Preview, Adobe Acrobat, and third-party Mac PDF readers.

## macOS-Specific Crash Causes

### Code Signing Issues
macOS Gatekeeper blocks unsigned or improperly signed PDFs, causing Preview to crash.

### Spotlight Indexing Conflicts
Spotlight trying to index corrupted PDFs causes system-wide slowdowns and crashes.

### Incompatible Font Rendering
PDFs with Windows-specific fonts crash macOS rendering engines.

## Preview App Fixes

**Reset Preview Preferences**:
```bash
killall Preview
rm ~/Library/Preferences/com.apple.Preview.plist
```

**Rebuild Preview Cache**:
```bash
rm -rf ~/Library/Caches/com.apple.Preview
```

**Repair Disk Permissions**:
```
Disk Utility → First Aid → Run on Macintosh HD
```

## Adobe Acrobat Mac Fixes

**Clear Adobe Cache**:
```bash
rm -rf ~/Library/Caches/com.adobe.Reader
rm ~/Library/Preferences/com.adobe.Reader.plist
```

**Reset Font Cache**:
```bash
atsutil databases -remove
```

**Reinstall Using App Cleaner**:
Download AppCleaner.app → Drag Adobe to it → Complete removal → Fresh install

## macOS System-Level Fixes

**Reset PRAM/NVRAM**:
```
Restart → Hold Cmd+Option+P+R until second startup chime
```

**Reset SMC** (Intel Macs):
```
Shut down → Shift+Control+Option+Power (10 seconds) → Release → Power on
```

**Check for macOS Updates**:
System Preferences → Software Update

## Best Mac PDF Readers (Crash-Free)

**PDF Expert** - $80/year, most stable professional option
**Skim** - Free, open-source, excellent for annotations
**PDFpen** - $75 one-time, editing + stability
**Foxit PDF Reader** - Free, cross-platform consistency

**Advanced help**: [Complete PDF Crash Guide](https://github.com/sendclickconvert/mrgrid-io/blob/main/articles/adobe-reader-keeps-crashing-when-opening-pdfs-here-s-how-to-fix-it-2025.md)