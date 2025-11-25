# Ansible Role for System File Hardening
**Author/Maintainer:** Josh Murphy

## Overview

This Ansible role automates hardening of the following system files:
```yaml
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
```

## Supported Platforms and Derivatives
The files changed should exist on every Redhat and Debian Distro. Below are the explicitly supported Distros.
```yaml
# RedHat
EL - All Versions
Fedora - All Versions
Rocky - All Versions
AlmaLinux - All Versions

# Debian
Debian - All Versions
Ubuntu - All Versions
```

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
```

This role was created and is maintained by **[CrowJM64](https://github.com/CrowJM64)**.