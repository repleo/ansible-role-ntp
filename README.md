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

The variables that can be passed to this role and a brief description about
them are as follows.

    ntp_timezone: /usr/share/zoneinfo/Europe/Amsterdam

    # in default cont, the ntp server will reply to time request, disable to reduce chance of being part of DDOS attacks
    ntp_serve_time: true


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
