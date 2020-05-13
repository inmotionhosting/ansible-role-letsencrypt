inmotionhosting.letsencrypt
=========

Modular Ansible Role for deploying and configuring Let's Encrypt

[![Build Status](https://travis-ci.org/inmotionhosting/ansible-role-letsencrypt.png?branch=master)](https://travis-ci.org/inmotionhosting/ansible-role-letsencrypt)

Requirements
------------

* CentOS 7.x or later
* Debian 9 or later
* Ubuntu 16.04.x LTS or later

Role Variables
--------------

| Variable | Description |
| -------- | ----------- |
| certbot_package | The Let's Encrypt certbot package.
| certbot_packages | Tools needed to verify if the usage of Let's Encrypt is valid.
| certbot_create_command | The command ran to generate a certificate.
| use_letsencrypt | Determines if Let's Encrypt should be installed/used.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: www
      roles:
         - role: inmotionhosting.letsencrypt

License
-------

GPLv3

Author Information
------------------

[InMotion Hosting](https://inmotionhosting.com)
