# Ansible Role: Certbot

[![Build Status](https://travis-ci.org/sbaerlocher/ansible.certbot.svg?branch=master)](https://travis-ci.org/sbaerlocher/ansible.certbot) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://sbaerlo.ch/licence) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-certbot-blue.svg)](https://galaxy.ansible.com/sbaerlocher/certbot)

## Description

Ansible role to install and configure letsencrypt with the certbot.

## Installation

```bash
ansible-galaxy install sbaerlocher.certbot
```

## Requirements

None

## Role Variables

### Certbot cloudflare

| Variable             | Default     | Comments (type)                                   |
| :---                 | :---        | :---                                              |
| certbot_binary_location | /usr/bin/certbot | |
| certbot_cron | false | creates an own cronjob for certbot |
| certbot_location | /etc/letsencrypt | |
| certbot_permissions_group | root | |
| certbot_permissions_mode | 0600 | |
| certbot_permissions_owner | root | |
| certbot_cloudflare_api_key | | Cloudflare account variables (must be set) |
| certbot_cloudflare_email | | Cloudflare account variables (must be set) |

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
     - sbaerlocher.certbot
```

## Changelog

### 1.2

* add Cloudflare DNS Support

### 1.1

* add Ubuntu Support
* clean role

### 1.0

* initial release

## Author

* [Simon Bärlocher](https://sbaerlocher.ch)

## License

This project is under the MIT License. See the [LICENSE](https://sbaerlo.ch/licence) file for the full license text.

## Copyright

(c) 2018, Simon Bärlocher