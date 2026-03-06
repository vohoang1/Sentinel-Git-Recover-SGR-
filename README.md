<img width="2640" height="1341" alt="Gemini_Generated_Image_vtqo0evtqo0evtqo" src="https://github.com/user-attachments/assets/411ed38e-f30d-4b92-9fcd-2a1e6d3c75f8" />

# Sentinel Git Recover (SGR)

<p align="center">
  <b>Advanced Git Repository Recovery & Forensic Toolkit</b>
</p>

<p align="center">
Recover lost commits, deleted branches, and corrupted Git repositories.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/python-3.9+-blue.svg">
  <img src="https://img.shields.io/badge/license-MIT-green.svg">
  <img src="https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Mac-lightgrey">
  <img src="https://img.shields.io/badge/status-active-success">
</p>

---

## Overview

**Sentinel Git Recover (SGR)** is a powerful forensic recovery toolkit designed to analyze, repair, and recover damaged or lost Git repository data.

The tool interacts directly with the Git object database and command-line interface, enabling advanced recovery capabilities beyond standard Git clients.

SGR can recover:

* Deleted commits
* Lost branches
* Orphan Git objects
* Stash entries
* Corrupted repository structures

It also provides forensic-level scanning of repository history.

---

## Key Features

### Repository Recovery

* Recover deleted commits
* Restore deleted branches
* Recover lost files from commit history
* Rebuild repository history

### Git Object Forensics

* Scan `.git/objects`
* Detect unreachable objects
* Analyze orphan commits
* Parse reflog history

### Repository Repair

* Detect corrupted objects
* Run repository integrity checks
* Repack and rebuild Git object database

### Automation

* Automatic recovery pipeline
* Multi-repository scanning
* Backup before recovery

### Developer Tools

* CLI interface
* Desktop GUI
* Portable Windows executable

---

## Supported Git Clients

SGR operates directly on Git repositories and works with any client built on Git including:

* SmartGit
* GitHub Desktop
* Sourcetree
* GitKraken
* Native Git CLI

---

## Project Architecture

```id="0p2udb"
sentinel-git-recover
│
├── main.py
├── gui.py
│
├── core
│   ├── recovery_engine.py
│   ├── object_scanner.py
│   ├── repo_repair.py
│
├── modules
│   ├── commit_recovery.py
│   ├── branch_recovery.py
│   ├── stash_recovery.py
│   ├── file_recovery.py
│
├── forensic
│   ├── orphan_scanner.py
│   ├── reflog_parser.py
│
├── plugins
│
├── logs
│
└── icon
    └── sgr.ico
```

---

## Installation

Clone the repository:

```id="ryoruj"
git clone https://github.com/your-username/sentinel-git-recover.git
```

Enter the project directory:

```id="nncytr"
cd sentinel-git-recover
```

Install dependencies:

```id="u2a9el"
pip install -r requirements.txt
```

---

## CLI Usage

Scan repository objects:

```id="h3sn9u"
python main.py --scan
```

Recover deleted commits:

```id="rqajaz"
python main.py --recover
```

Run automatic recovery:

```id="x9j7q6"
python main.py --auto
```

---

## Building Portable Executable

Install PyInstaller:

```id="1p0dfc"
pip install pyinstaller
```

Build executable:

```id="9xj08m"
pyinstaller --onefile --name "Sentinel Git Recover (SGR)" main.py
```

Output:

```id="wsc8u6"
dist/Sentinel Git Recover (SGR).exe
```

---

## Example Workflow

Typical recovery process:

1. Backup repository
2. Scan Git objects
3. Detect unreachable commits
4. Restore lost branches
5. Rebuild repository database

---

## Roadmap

Future development goals:

* Deep Git object recovery
* Disk-level repository scanning
* AI-assisted commit reconstruction
* Enterprise DevOps recovery features
* Advanced repository forensic analysis

---

## Contributing

Contributions are welcome.

Steps:

1. Fork the repository
2. Create a new feature branch
3. Commit changes
4. Submit a pull request

---

## Security

SGR follows safe recovery practices:

* Read-only scanning by default
* Automatic repository backup
* Explicit confirmation for write operations

---

## License

MIT License

---

## Author

Vo Dinh Hoang
Thủ Đức College of Technology

---

## Disclaimer

This software is intended for repository recovery, research, and educational purposes.

Always create backups before performing recovery operations.
