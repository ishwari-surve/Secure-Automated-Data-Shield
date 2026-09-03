# 🛡️ Secure Automated Data Shield

> Intelligent automated backup system with smart change detection, 
> scheduled execution, and secure archiving.

A Python-based backup automation tool that intelligently identifies and backs up 
only new or modified files, eliminating redundant copying and saving storage space.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔐 **Smart Backup** | Copies only new & modified files using MD5 checksum |
| 📦 **Auto Compression** | Creates timestamped ZIP archives automatically |
| ⏰ **Scheduled Execution** | Runs at user-defined intervals (background process) |
| 🛡️ **Data Integrity** | Preserves file metadata & folder structure |
| 🎯 **CLI Support** | Simple command-line interface for easy operation |

---

## 🚀 Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Start backup (every 5 minutes)
python src/secure_backup.py 5 Data

# Get help
python src/secure_backup.py --h
```

---

## 📋 Installation

### Clone Repository
```bash
git clone https://github.com/YourUsername/secure-automated-data-shield.git
cd secure-automated-data-shield
```

### Install Requirements
```bash
pip install -r requirements.txt
```

Or manually:
```bash
pip install schedule
```

---

## 💻 Usage

### Display Help
```bash
python src/secure_backup.py --h
```
Shows project description and available options.

### Display Usage Format
```bash
python src/secure_backup.py --u
```
Shows command-line syntax.

### Start Backup
```bash
python src/secure_backup.py 5 Data
```

**Parameters:**
- `5` → Backup interval (minutes)
- `Data` → Source directory to backup

---

## 📊 How It Works
```bash
Step 1: User runs script with time interval & source folder
↓
Step 2: Application creates backup folder (if doesn't exist)
↓
Step 3: Scheduler registers periodic backup job
↓
Step 4: Every N minutes:
├─ Scans source directory recursively
├─ Compares MD5 checksums (source vs backup)
├─ Copies only NEW or MODIFIED files
├─ Creates timestamped ZIP archive
└─ Logs backup report
↓
Step 5: Archives accumulate for version history
```

---

## 📄 Sample Output
```bash
-------Secure Automated Data Shield--------

Inside projects logic
Time interval: 5
Directory name: Data

Data Shield System started successfully
Time interval in minutes : 5
Press Ctrl + C to Stop the execution

Backup Process Started successfully at: Thu Sep 04 14:25:30 2026
Creating the Backup folder for backup process
Report about the backup
documents/report.pdf
images/photo.jpg
config/settings.txt

Backup completed successfully
Files copied: 3
Zip file created: SecureBackup_2026-09-04_14-25-30.zip
```
---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Python 3.x** | Core language |
| **schedule** | Job scheduling |
| **hashlib** | MD5 checksum calculation |
| **zipfile** | Archive creation |
| **shutil** | File operations |
| **os** | Directory management |

---

## 📁 Project Structure
```
secure-automated-data-shield/
│
├── src/
│ └── secure_backup.py # Main application
│
├── docs/
│ ├── SETUP.md # Installation guide
│ ├── USAGE.md # Detailed usage
│ └── ARCHITECTURE.md # Technical details
│
├── examples/
│ └── sample_data/ # Test data
│
├── tests/
│ └── test_backup.py # Unit tests
│
├── logs/ # Auto-generated backups
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## 🎯 Key Concepts Demonstrated

✅ Python Automation & Scripting  
✅ File System Operations  
✅ Cryptographic Hashing (MD5)  
✅ Archive/Compression (ZIP)  
✅ Job Scheduling  
✅ Command-Line Interface  
✅ Incremental Backups  
✅ Exception Handling  
✅ Data Integrity Checks  

---

## 💡 Use Cases

- Critical document protection
- Database backup automation
- Development project versioning
- Media file archival
- Continuous data safety
- Scheduled daily backups

---

## 🔮 Future Enhancements

- [ ] Email alerts for backup completion
- [ ] PDF report generation
- [ ] CSV export for analysis
- [ ] Real-time dashboard
- [ ] GUI with Tkinter
- [ ] Database storage (SQLite)
- [ ] Cloud backup integration
- [ ] Process filtering
- [ ] Resource threshold alerts
- [ ] Automatic cleanup of old backups

---

## ⚙️ Requirements

- Python 3.6+
- pip (package manager)
- Windows / Linux / macOS
- Disk space for backups

---

## 📝 Command-Line Reference

| Command | Purpose |
|---------|---------|
| `--h` or `--H` | Display help information |
| `--u` or `--U` | Display usage format |
| `interval` | Backup interval (minutes) |
| `directory` | Source directory name |

---

## 🐛 Troubleshooting

**Problem:** "No such file or directory"
```bash
# Solution: Create data folder first
mkdir Data
```

**Problem:** "Permission denied"
```bash
# Solution: Run with appropriate permissions
sudo python src/secure_backup.py 5 Data
```

---

## 👤 Author

**Ishwari Vijaykumar Surve**  


