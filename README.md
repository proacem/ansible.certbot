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

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
     - sbaerlocher.certbot
```

## Changelog

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

(c) 2016, Simon Bärlocher