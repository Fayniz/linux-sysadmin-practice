This repo tracks my learning and practical exercises to build Linux system administration skills. The goals are to practice user management, services, security hardening, networking and scripting.

### User Management
- Created a new Linux user 'testuser' using:
  ```bash
  sudo adduser testuser
  sudo usermod -aG sudo testuser

* Saved terminal history to 'adduser-commands.txt'

### Service Management

* Managed services using `systemctl`:

  ```bash
  systemctl status cron
  sudo systemctl stop cron
  sudo systemctl start cron
  sudo systemctl disable cron
  sudo systemctl enable cron
  ```
* Saved terminal history to 'service-management.txt'

### Permission Management

* Practiced file permission and ownership:

  ```bash
  touch file.txt
  sudo chown testuser file.txt
  chmod 600 file.txt
  ```
* Saved terminal history to 'Permissions.txt'

### Scripting and Automation

* Created bash script to delete `.tmp` files from `/tmp`:

  ```bash
  echo -e '#!/bin/bash\nrm -f /tmp/*.tmp' > cleanup.sh
  chmod +x cleanup.sh
  ./cleanup.sh
  ```
* Saved terminal history to 'create-script-file.txt'

### System Monitoring

* Explored disk and memory usage:

  ```bash
  df -h
  du -sh ~
  free -h
  ```
* Saved terminal history in 'disk-memory.txt'

### SSH

* Generated RSA SSH key pair:

  ```bash
  ssh-keygen -t rsa -b 4096 -C "fayyadhnizar@gmail.com"
  cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
  ```
* Disabled root SSH login by editing `/etc/ssh/sshd_config`
* Tested SSH key login to localhost:

  ```bash
  ssh root@localhost
  ```
* Saved terminal history in 'ssh-key-setup.txt'

### Firewall 

* Installed UFW:

  ```bash
  sudo apt install ufw
  ```
* Set default policies and allowed ports:

  ```bash
  sudo ufw default deny incoming
  sudo ufw default allow outgoing
  sudo ufw allow ssh
  sudo ufw allow 80/tcp
  sudo ufw allow 443/tcp
  sudo ufw enable
  sudo ufw status verbose
  sudo fail2ban-client status
  ```
* Saved terminal history in 'firewall-setup.txt'
