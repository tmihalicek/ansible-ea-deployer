# ansible-ea-deployer
Deployment of elastic agent via ansible.

# Ansible Role: ea-deployer

Installs elastic-agent on Linux.

## Requirements

None.

## Role Variables

## Example Playbook

    - hosts: elastic_agent_clients
      roles:
        - { role: "role/ea-deployer" }

*Inside `role/ea-deployer/vars/main.yml`*:

    elastic_agent_version: 8.2.3

## Author Information

This role was created in 2022 by [Tomislav Mihalicek](https://tmihalicek.github.io/).

