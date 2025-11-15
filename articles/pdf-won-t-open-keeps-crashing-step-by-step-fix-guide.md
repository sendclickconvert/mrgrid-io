# PDF Won't Open Keeps Crashing - Step-by-Step Fix Guide

# PDF Won't Open Keeps Crashing - Step-by-Step Fix Guide

**PDF crashes immediately on open?** This systematic troubleshooting guide diagnoses and fixes instant-crash issues across all PDF readers.

## Instant Crash Diagnosis

### Crash Timing Analysis
- **0-1 seconds**: Application launch failure (corrupted install)
- **1-3 seconds**: File parsing failure (corrupted PDF header)
- **3-5 seconds**: Rendering failure (graphics driver issue)

### Error Message Decoding

| Error | Cause | Fix |
|-------|-------|-----|
| "Failed to load document" | Corrupted PDF structure | Repair with QPDF |
| "Access violation" | Graphics driver conflict | Update GPU drivers |
| "Out of memory" | Insufficient RAM | Close other apps |
| No error (silent crash) | Background process kill | Check Task Manager |

## Step-by-Step Fix Protocol

**Step 1: Test File Integrity**
```bash
qpdf --check suspicious.pdf
```

**Step 2: Try Alternative Reader**
Chrome browser (drag and drop PDF) → If opens, Adobe is the problem

**Step 3: Disable Hardware Acceleration**
Edit → Preferences → Page Display → Uncheck "Use 2D graphics acceleration"

**Step 4: Clear Reader Cache**
Windows: Delete %AppData%\Adobe\Acrobat
Mac: Delete ~/Library/Caches/com.adobe.Reader

**Step 5: Repair or Reinstall**
Use Adobe's official Cleaner Tool for complete removal, then fresh install

## Advanced Troubleshooting

**Safe Mode Boot**: Tests if third-party software conflicts
**Event Viewer Analysis** (Windows): eventvwr.msc → Application logs
**Console.app Logs** (Mac): Filter for "PDF" or "Adobe" crashes

**Get expert help**: [AI Debugger](/ai-debugger) | [Live Support](https://afflat3d3.com/trk/lnk/0B2305B4-17D5-4967-B19A-AB86DEA4FA70/?o=21413&c=918277&a=620195&k=8B02443E8F32B5B6A73ACC66DFA99EEC&l=22313)