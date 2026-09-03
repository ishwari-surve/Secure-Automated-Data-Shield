# Setup Guide

## Installation

### Prerequisites
- Python 3.6 or higher
- pip (Python package manager)

### Step 1: Clone Repository

```bash
git clone https://github.com/YourUsername/Secure-Automated-Data-Shield.git
cd Secure-Automated-Data-Shield
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

Or manually:
```bash
pip install schedule
```

### Step 3: Create Data Folder (Optional)

```bash
mkdir Data
```

### Step 4: Run the Script

```bash
python src/secure_backup.py 5 Data
```

## Troubleshooting

**Problem:** "No module named schedule"
```bash
pip install schedule
```

**Problem:** "No such file or directory"
```bash
mkdir Data
```

**Problem:** "Permission denied"
```bash
# On Linux/Mac
sudo python src/secure_backup.py 5 Data
```

## System Requirements

- Windows 7+
- Linux (any distribution)
- macOS 10.12+
- Disk space for backups
