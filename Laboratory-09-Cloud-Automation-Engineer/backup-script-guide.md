# Backup Script Guide

## 1. Introduction

This guide explains how to create and execute a Bash backup script and schedule it using Linux Cron. The script compresses the `app-data` directory into a `.tar.gz` archive stored in the `backups` directory.

## 2. Full Bash Script

The following is the complete code used for `backup.sh`.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. Explanation of the Script

- `#!/bin/bash` specifies Bash as the script interpreter.
- `SOURCE_DIR="app-data"` identifies the directory to back up.
- `BACKUP_DIR="backups"` identifies the directory where backups will be stored.
- `TIMESTAMP=$(date +"%Y%m%d_%H%M%S")` generates a date and time for the backup filename.
- `echo` displays messages in the terminal.
- `mkdir -p` creates the backup directory if it does not already exist.
- `tar -czf` creates a compressed archive of the source directory.

Each backup receives a timestamped filename, helping distinguish different backup versions.

## 4. File Permissions Using chmod

The command used was:

```bash
chmod +x backup.sh
```

The `chmod` command changes file permissions, while `+x` adds execute permission. This allows the script to be run directly using `./backup.sh`.

Before adding execute permission, running the script directly may produce a `Permission denied` error.

## 5. Testing the Backup

The following commands were used to create and verify the backup:

```bash
./backup.sh
ls -l backups/
tar -tzf backups/*.tar.gz
```

The `ls -l backups/` command lists the generated archive. The `tar -tzf` command displays the contents of the compressed backup without extracting it.

## 6. Cron Job Configuration

The Cron expression used was:

```cron
0 2 * * * /root/backup.sh
```

This schedules the script to run every day at 2:00 AM, provided the system and Cron service are running.

### Breakdown of the Five Cron Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The final part, `/root/backup.sh`, is the absolute path to the script.

To edit and verify the schedule, the following commands were used:

```bash
env EDITOR=nano crontab -e
crontab -l
```

The `crontab -l` command displays the installed Cron schedule.

## 7. Conclusion

Bash scripting and Cron help automate repetitive tasks and reduce the need for manual administration. Testing the script, verifying backup archives, and checking the Cron configuration are important steps in maintaining reliable automated backups.

