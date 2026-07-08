# Ansible Learning Project

This project was created to learn Ansible basics.

## Infrastructure

AWS EC2 Ubuntu instance

## Ansible structure

- inventory.ini - contains managed hosts
- playbook.yml - main automation scenario
- roles/server_setup - server configuration tasks

## Current automation

The playbook:
- connects to AWS EC2 via SSH
- updates apt cache
- installs htop

## Run

ansible-playbook -i inventory.ini playbook.yml
