# Uptime Kuma (Ansible)

[![Ansible Lint](https://github.com/leberkaslabs/ansible-uptimekuma-deployment/actions/workflows/ansible-lint-action.yml/badge.svg)](https://github.com/leberkaslabs/ansible-uptimekuma-deployment/actions/workflows/ansible-lint-action.yml)

This repository contains Ansible playbooks to fully automate the deployment of Uptime Kuma in Docker, including optional setup of an NGINX reverse proxy for secure access.

## Prerequisites

- Ensure you have Ansible installed (e.g. `pip3 install ansible`)
- Ensure Docker is installed (you may want to checkout my [ansible-docker-role](https://github.com/DudeCalledBro/ansible-role-docker))

## Usage

Before running the playbooks, prepare the inventory and configuration files.

1. Copy the example inventory file to `hosts.yml`:

    ```bash
    cp inventories/hosts.example.yml inventories/hosts.yml
    ```

2. Run the Ansible playbook:

    ```bash
    ansible-playbook main.yml
    ```

## License

Copyright (c) 2026 Niclas Spreng
