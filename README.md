Ansible Role: ntpd
=========

[![Build Status](https://travis-ci.org/fahlke/ansible-role-ntpd.svg?branch=master)](https://travis-ci.org/fahlke/ansible-role-ntpd)

Installs ntpd on Debian or Ubuntu.

Requirements
------------

None.

Installation
------------

    ansible-galaxy install fahlke.ntpd

Role Variables
--------------

Available variables are listed below, along with default values (see ```defaults/main.yml```):

**TODO(fahlke): Add documentation**

    ntpd_cfg_...

→ []()

Dependencies
------------

None.

Example Playbook
----------------

Installing the role on all hosts with the default configuration.

    - hosts: all
      roles:
         - { role: fahlke.ntpd }

License
-------

MIT

Author Information
------------------

This role was created in 2017 by Alexander Fahlke.

Important Notes/Caveats
-----------------------
- currently installs ntpd only on Debian and Ubuntu
