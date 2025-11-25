# Ansible Role for System File Hardening
**Creator:** Josh Murphy

## Overview

This Ansible role automates hardening of the following system files:

- /boot
- /etc/cron.monthly
- /etc/cron.weekly
- /etc/cron.daily
- /etc/cron.hourly
- /etc/crontab
- /etc/ssh/sshd_config
- /etc/passwd
- /etc/group
- /etc/shadow
- /etc/gshadow
- /run/shm
- /dev/shm


## Supported Platforms



## Example Playbook

```yaml
- hosts: all
  become: yes

  roles:
    - role: system_file_hardening
```

### From Ansible Galaxy

```bash
ansible-galaxy install crowjm64.system_file_hardening

## Author
**Josh Murphy**
Infrastructure Engineer - Learning Every Day