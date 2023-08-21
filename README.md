![Ansible Molecule Pipeline](https://github.com/inmotionhosting/ansible-role-letsencrypt/actions/workflows/main.yml/badge.svg) [![GPL-3.0 License](https://img.shields.io/github/license/inmotionhosting/ansible-role-letsencrypt.svg?color=blue)](https://github.com/inmotionhosting/ansible-role-letsencrypt/blob/master/LICENSE) [![GitHub stars](https://img.shields.io/github/stars/inmotionhosting/ansible-role-letsencrypt.svg)](https://github.com/inmotionhosting/ansible-role-letsencrypt/stargazers)

# Ansible Role: Let's Encrypt

Modular Ansible Role for deploying and configuring Let's Encrypt

## Requirements
This Ansible role supports the two latest stable releases of specific
server-focused Linux distributions and aims to follow their deprecation
policies. Additionally we will focus on supporting the latest two stable
releases of each, which at the time of writing are as follows:

* CentOS 7.x
* Debian 10 or later
* Ubuntu 20.04 LTS or later
* AlmaLinux 8.x or later
* RockyLinux 8.x or later

## Dependencies

community.crypto

## Role Variables

Available variables are listed below with their default values (you can also see `defaults/main.yml`)

| Variable | Description |
| -------- | ----------- |
| certbot_package | The Let's Encrypt certbot package.
| certbot_packages | Tools needed to verify if the usage of Let's Encrypt is valid.
| certbot_create_command | The command ran to generate a certificate.
| use_letsencrypt | Determines if Let's Encrypt should be installed/used.
| certbot_test_cert | Use Letsencrypt Staging Environment
| certbot_without_email | Register Letsencrypt account without an email

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
