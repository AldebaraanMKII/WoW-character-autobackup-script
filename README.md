# WoW-character-autobackup-script
This needs my backup/restore scripts: https://github.com/AldebaraanMKII/WoW-character-and-guild-export-import-scripts

# Configuration
$CharacterList = List of characters that you want to backup. Case sensitive.
$BackupDelay = backup the characters every $BackupDelay seconds.
$7zipCompression = Create a 7z archive and then delete the folder to save space.
$DBFilePath = No need to mess with this.

# Usage
1. Clone this and my backup/restore scripts. Make sure they are in the same folder.
2. Configure "(Config) Backup scripts.ps1"
3. Configure "(Config) AutoBackup script.ps1"
4. Open the database your characters are in
5. Run the script: .\"Autobackup script.ps1"

# FAQ
Q: Can i play while this runs?
A: Yes. It was my intention to backup the characters while they are being played.

Q: I set it to backup every X seconds but they only backup several tries later!
A: Worldserver.conf PlayerSaveInterval needs to be edited. Set it to something lower than what you set $BackupDelay.
