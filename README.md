#Linux Sysadmin Practice

This repo tracks my learning and practical exercises to build Linux system administration skills. The goals are to practice user manangement, services, security hardening, networking and scripting.

## Day 1 (14 July)
- Created a new Linux user 'testuser' using 'adduser'
- Added the user to the 'sudo' with 'usermod -aG'
- Saved terminal history to 'adduser-commands.txt'

## Day 2 (15 July)
- Manage service using 'systemctl'
- Checked, stopped, started, disabled, enabled, cron service
- Saved terminal history to 'service-management.txt'

## Day 3 (16 July)

- Practiced file permission and ownership using 'chmod' and 'chown'
- Created a test file, changed ownership to 'testuser'
- Restricted file access to owner only with 'chmod 600'
- Saved terminal history to 'Permissions.txt'

## Day 4 (17 July)

- Create bash script file to delete '.tmp' files from '/tmp'
- Made the script executable using 'chmod +x' 
- Ran the script succesfully
- Saved terminal history to 'create-script-file.txt'

## Day 5 (18 July)

- Explored disk space using 'df -h' and directory usage 'du -sh'
- Checked memory status with 'free -h' and understood Linux memory usage
- Learned the difference between RAM and disk storage
- Saved terminal history in 'disk-memory.txt'

## Day 6 (19 July)

- Generated RSA SSH key pair with 4096-bit encryption
- Added public key to ~/.ssh/authorized_keys for passwordless SSH login
- Disabled root login via SSH for better security
- Tested SSH key login to localhost with no password prompt
- Saved terminal history in 'ssh-key-setup.txt' 
