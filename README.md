This repo tracks my learning and practical exercises to build Linux system administration skills. The goals are to practice user management, services, security hardening, networking and scripting.

### User Management
* Created new users, assigned groups and sudo rights
* Managed file ownership and permissions with chown and chmod
* Saved terminal history to 'adduser-commands.txt'

### Service Management

* Managed services using `systemctl`:
* Used systemctl to start, stop, enable, disable services
* Explored logs with journalctl
* Saved terminal history to 'service-management.txt'

### Permission Management

* Practiced file permission and ownership
* Created a test file, changed ownership to 'testuser'
* Restricted file access to owner only with `chmod 600`
* Saved terminal history to 'Permissions.txt'

### Scripting and Automation

* Created bash script to delete `.tmp` files from `/tmp`
* Made the script executable using `chmod +x` 
* Ran the script succesfully
* Saved terminal history to 'create-script-file.txt'

### System Monitoring

* Explored disk space using `df -h` and directory usage `du -sh`
* Checked memory status with `free -h` and understood Linux memory usage
* Learned the difference between RAM and disk storage
* Saved terminal history in 'disk-memory.txt'

### SSH

* Generated RSA SSH key pair with 4096-bit encryption
* Added public key to `~/.ssh/authorized_keys` for passwordless SSH login
* Disabled root login via SSH for better security
* Tested SSH key login to localhost with no password prompt
* Saved terminal history in 'ssh-key-setup.txt'

### Firewall 

* Installed and configured ufw for system security
* Set default policies to deny all incoming and allow all outgoing traffic
* Allowed necessary ports: SSH(22), HTTP(80), and HTTPS(443)
* Enabled firewall and verify status
* Understand the importance of security
* Saved terminal history in 'firewall-setup.txt'

### IP addressing and Routing

* Learned interface, local IP, gateway
* Routing checked with `ip r`
* Understood default route and local subnet
* Saved terminal output in 'ip-routing.txt'

### DNS Queries and Domain Lookup

* Practiced using `dig` to query A and MX records for domains
* Used `dig +shorts` to get clean IP output
* Queried authoritative nameservers with `nslookup -type=NS`
* Observed response secitons, query time and DNS server used
* Learned difference between A, MX and NS record type
* Saved terminal output in 'dns-lookup.txt'

### Web server setup (Apache)
* Installed Apache
* Located the default web root /var/www/html
* Verified local web server is running: opened `http://localhost`
* Saved terminal history in 'Apache-web-server-setup.txt'

### Virtual Host Setup with Apache

* Created a new directory `/var/www/fayyadh.test` to host a custom website
* Used `chown` to give current user permission to manage the directory
* Moved a sample `index.html` file into the site folder
* Created a virtual host config file in `/etc/apache2/sites-available/fayyadh.test.conf`
* Enabled the site using `a2ensite` and reloaded Apache to apply the changes
* Edited `/etc/hosts` to resolve `fayyadh.test` to `127.0.0.1`
* Verified that the custom web page loads successfully at `http://fayyadh.test`
* Saved terminal history at 'virtual-host.txt'
