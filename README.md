# Ansible Role: Plantd Master

<!--[![Build Status](https://img.shields.io/travis/geoffjay/ansible-plantd-broker/master.svg?style=flat)](https://travis-ci.org/geoffjay/ansible-plantd-broker-->
<!--[![stability-stable](https://img.shields.io/badge/stability-stable-green.svg?style=flat)](https://github.com/orangemug/stability-badges)-->
[![Ansible Galaxy](https://img.shields.io/ansible/role/36029.svg?style=flat)](https://galaxy.ansible.com/geoffjay/plantdbroker)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://raw.githubusercontent.com/geoffjay/ansible-plantd-broker/master/LICENSE)

[WIP] Pre-alpha, doesn't work.

Installs and configures a Plantd broker server on a Debian host.

## Requirements

A working installation of `go`.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yml
plantd_broker_version: "0.1.0"
```

## Dependencies

None

## Example Playbook

```yml
- hosts: master
  become: yes
  vars_files:
    - vars/main.yml
  roles:
    - geoffjay.plantdbroker
```

Inside `vars/main.yml`:

```yml
plantd_broker_version: "0.1.0"
```

## License

MIT/BSD

## Author Information

This role was created in 2019 by Geoff Johnson.
