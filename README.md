Ansible role - NTP client configuration and monitor cronjob
=====

[![Build Status](https://travis-ci.org/repleo/ansible-role-ntp.svg?branch=master)](https://travis-ci.org/repleo/ansible-role-ntp)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-repleo.ntp-660198.svg?style=flat)](https://galaxy.ansible.com/repleo/ntp)

This role configures NTP. It also installs a cronjob to check if NTP is still working properly.
This is mainly an issue when running an NTP client on a virtual machine.

Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements are listed in the metadata file.

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

Install ntp
```yaml
- hosts: all
  roles:
    - { repleo.ntp }
```

License
-------

GPL v3 - (c) 2016, Repleo, Amstelveen

Author Information
------------------

Repleo, Amstelveen, Holland -- www.repleo.nl  
Jeroen Arnoldus (jeroen@repleo.nl)


