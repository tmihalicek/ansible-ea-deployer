# ansible-ea-deployer
Deployment of elastic agent via ansible.

# Ansible Role: ea-deployer

Installs elastic-agent on Linux.

## Requirements

None.

## Role Variables

## Example Playbook

    - hosts: all
      roles:
        - geerlingguy.ntp

*Inside `role/ea-deployer/vars/main.yml`*:

    ntp_timezone: Europe/Zagreb

## Author Information

This role was created in 2022 by [Tomislav Mihalicek](https://tmihalicek.github.io/).

