[![Build Status](https://travis-ci.org/inmotionhosting/ansible-role-letsencrypt.png?branch=master)](https://travis-ci.org/inmotionhosting/ansible-role-letsencrypt) [![GPL-3.0 License](https://img.shields.io/github/license/inmotionhosting/ansible-role-letsencrypt.svg?color=blue)](https://github.com/inmotionhosting/ansible-role-letsencrypt/blob/master/LICENSE) [![GitHub stars](https://img.shields.io/github/stars/inmotionhosting/ansible-role-letsencrypt.svg)](https://github.com/inmotionhosting/ansible-role-letsencrypt/stargazers)

# Ansible Role: Let's Encrypt

Modular Ansible Role for deploying and configuring Let's Encrypt

## Requirements

* CentOS 7.x or later
* Debian 9 or later
* Ubuntu 16.04 LTS or later

## Dependencies

None.

## Role Variables

Available variables are listed below with their default values (you can also see `defaults/main.yml`)

| Variable | Description |
| -------- | ----------- |
| certbot_package | The Let's Encrypt certbot package.
| certbot_packages | Tools needed to verify if the usage of Let's Encrypt is valid.
| certbot_create_command | The command ran to generate a certificate.
| use_letsencrypt | Determines if Let's Encrypt should be installed/used.

## Example Playbook

```yaml
- hosts: www
  roles:
    - role: inmotionhosting.letsencrypt
```

## License

GPLv3

## Author Information

[InMotion Hosting](https://inmotionhosting.com)
