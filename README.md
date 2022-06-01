## Ansible  LEMP stack  on Debian 11
This playbook will install  **LEMP Stack** on debian 11. To run this script you need to have a fresh VPS with debian 11 installed. The minimum hardware requirements for the server is:
**CPU:** 2 vCores or more
**RAM:** 2 Gigabytes or more
**DISK:** 20 Gigabytes or more

### Here is the version information:
**Nginx: ** 1.18.0
**MariaDB: ** 10.5.15
**PHP: ** 8.1.6

### Settings in group_vars/all:
**hostname: ** Domain name or server name (in this case: example.com)
**project_name: ** A directory will be created with this name in: /var/www/
**nginx_port: ** nginx will listen on this port
**mysql_root_password:  **The password for the MySQL root account.

### Run the Playbook:
```
ansible-playbook -l [target] -i [inventory file] -u [remote user] lemp.yml
```
