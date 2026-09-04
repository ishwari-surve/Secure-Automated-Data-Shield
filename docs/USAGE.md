# Usage Guide

## Quick Start

Run the script to backup every 5 minutes:

```bash
python src/secure_backup.py 5 Data
```

## Command Syntax

```bash
python src/secure_backup.py TimeInterval SourceDirectory
```

### Parameters

- **TimeInterval**: Backup interval in minutes (e.g., 5, 10, 30)
- **SourceDirectory**: Folder name to backup (e.g., Data, Documents)

---

## Examples

### Example 1: Backup every 5 minutes

```bash
python src/secure_backup.py 5 Data
```

### Example 2: Backup every 10 minutes

```bash
python src/secure_backup.py 10 Documents
```

### Example 3: Backup every 1 minute (testing)

```bash
python src/secure_backup.py 1 Data
```

---

## Help Commands

### Display Help Information

```bash
python src/secure_backup.py --h
```

Shows what the script does and its features.

### Display Usage Format

```bash
python src/secure_backup.py --u
```

Shows command syntax and parameters.

---

## What Happens

When you run the script:

1. **Creates SecureBackup folder** — Copies files from source
2. **Scans for changes** — Uses MD5 checksum to detect modifications
3. **Copies only new/modified files** — Saves time and storage
4. **Creates ZIP archive** — Timestamped compressed file
5. **Runs on schedule** — Repeats every N minutes
6. **Prints status** — Shows progress in terminal

---

## Output Example
```bash
----------Secure Automated Data Shield-----------

Inside project logic
Time interval : 5
Directory Name : Data

Data Shield System started successfully
Time Interval in minutes : 5
Press CTRL + C to stop the execution
Backup Process Started Successfully at : Thu Sep 04 14:30:00 2026
Creating the Backup folder for backup process
Backup Completed Successfully
Files Copied : 2
Zip Files created : SecureBackup_2026-09-04_14-30-00.zip
```

---

## Generated Files

After running, you'll see:

- **SecureBackup/** — Backup folder with copied files
- **SecureBackup_YYYY-MM-DD_HH-MM-SS.zip** — Compressed archive with timestamp

---

## Stopping the Script

Press: **Ctrl + C**

This stops the scheduled backups.

---

## File Structure During Backup
```bash
Project Root/
│
├── Data/ (Your source files)
│ ├── file1.txt
│ └── file2.txt
│
├── SecureBackup/ (Generated backup)
│ ├── file1.txt
│ └── file2.txt
│
└── SecureBackup_2026-09-04_14-30-00.zip (Generated archive)

```

---

## Features in Action

✅ **Smart Detection** — Only copies files that changed  
✅ **Compression** — Saves disk space with ZIP  
✅ **Timestamps** — Tracks when each backup ran  
✅ **Automatic** — Runs without manual intervention  
✅ **Recursive** — Backs up subfolders too  

---

## Troubleshooting

**Issue:** Script stops immediately

**Solution:** Make sure `Data` folder exists with files inside

---

**Issue:** "Can't find src/secure_backup.py"

**Solution:** Run from project root, not from src/ folder

---

**Issue:** No files copied

**Solution:** Check if files in Data/ folder are actually new or modified

---


