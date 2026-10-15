# Laboratory Activity 9: The Cloud Automation Engineer

## Mission Overview

This laboratory activity focuses on automating cloud administration tasks using Bash scripting and Linux Cron. I created a Bash script that compresses application data into a `.tar.gz` backup file and configured a Cron job to schedule the backup every day at 2:00 AM.

## Objectives

- Understand the fundamentals of Bash shell scripting.
- Create and execute an automated backup script.
- Modify file permissions using the `chmod` command.
- Configure scheduled tasks using Linux Cron.
- Document automation procedures using Markdown.
- Complete the ninth laboratory activity in the Cloud Computing portfolio.

## Commands Executed

### Create Application Data

```bash
mkdir -p app-data
echo "This is critical client data." > app-data/data.txt
```

### Create and Execute the Script

```bash
nano backup.sh
chmod +x backup.sh
./backup.sh
```

### Verify the Backup

```bash
ls -l backups/
tar -tzf backups/*.tar.gz
```

### Configure the Cron Job

```bash
env EDITOR=nano crontab -e
crontab -l
```

### Cron Schedule


