ansible-centos-init-system-env
===========

This role help to init CentOS/RH system

including:

*  bash
*  timezone
*  limits
*  files
*  sudo
*  hosts
*  disable-selinux
*  disable-networkmanager
*  yum install common packages


Usage
-----

```
---
- hosts: localhost
  connection: local
  roles:
    - role: ansible-centos-init-system-env

      set_bash: true
      set_timezone: true
      set_limits: true
      set_files: true
      set_sudo: true
      set_hosts: false
      disable-selinux: true
      disable-networkmanager: true
      yum_install_common_package: true

      timezone: 'Asia/Shanghai'
```
