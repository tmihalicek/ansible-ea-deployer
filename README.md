# ansible-ea-deployer
Deployment of elastic agent via ansible.

# Ansible Role: ea-deployer

Installs elastic-agent on Linux.

## Requirements

None.

## Role Variables

## Example Playbook

    - hosts: elastic_agent_clients
      gather_facts: true
      vars_prompt:
        - name: "elastic_agent_version"
          prompt: "Enter elastic agent version."
          private: no
          default: "{{ elastic_agent_version }}"
        - name: "fleet_url"
          prompt: "Enter fleet url."
          private: no
          default: "{{ fleet_url }}"
        - name: "fleet_token"
          prompt: "Enter fleet token."
          private: yes
      roles:
        - { role: "role/ea-deployer" }

*Inside `role/ea-deployer/vars/main.yml`*:

    elastic_agent_version: 8.2.3
    fleet_url: https://kibana.domain.org:8220

## Author Information

This role was created in 2022 by [Tomislav Mihalicek](https://tmihalicek.github.io/).

