# Disk Space Monitoring Script

This Bash script is designed to monitor the free filesystem space on your system and send an email alert if the available disk space falls below a certain threshold.

## Prerequisites

- This script relies on the `mail` command for sending email alerts, so make sure you have a working email configuration. It is recommended to use the "Postfix" mail server.

## Installation Steps for Postfix

1. Ensure that you have administrative privileges to install and configure software on your system.

2. Install Postfix using your package manager. The commands may vary based on your Linux distribution:

   For Debian/Ubuntu:
   ```bash
   sudo apt-get install postfix

  During the installation, you'll be prompted to configure Postfix. To do so:

1. Select "Internet Site" when prompted.
2. Enter your system's domain name when prompted.

## Script Configuration

Open the script and configure the following variables:
- `TO`: Specify the recipient email address where you want to receive disk space alerts.
The script will check the disk space, and if it's below the threshold (20% by default), it will send an email alert.

# Notes
You should ensure that the mail command is properly configured on your system to send emails. If you encounter issues with the mail command, consult your system's email configuration and consider using alternative methods for sending alerts.

This script is intended for monitoring disk space and sending alerts. You can customize the threshold and alert message to fit your specific needs.
## Running the Script

Run the script using the Bash shell:

```bash
bash disk_space_monitor.sh
