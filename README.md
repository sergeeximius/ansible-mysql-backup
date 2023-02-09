mysql-backup
=========

Install and configure script for automated backups of MySQL Databases https://github.com/sixhop/AutoMySQLBackup

Requirements
------------

Debian/Ubuntu only

Role Variables
--------------
```
mysql_backup_dbhost: "localhost"
mysql_backup_dbuser: "root"
mysql_backup_dbpassword: "StrongPassword"
mysql_backup_destination_dir: "/mnt/backup/mysql"
```

Dependencies
------------

None

Example Playbook
----------------

requirements.yml
```
---
roles:
  - src: https://github.com/sergeeximius/ansible-role-mysql-backup.git
    scm: git
    name: sergeeximius.mysql-backup
```

playbook.yml
```
---
- hosts: servers
  roles:
    - role: sergeeximius.mysql-backup
```
License
-------

BSD

Author Information
------------------

Sergey Sedov serge.eximius@gmail.com
