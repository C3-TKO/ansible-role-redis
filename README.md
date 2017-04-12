# ansible-role-redis

This is an Ansible role for installing and configuring redis-server packages on a rapsberry pi. Redis will common with standard configuration. As this role is meant to be used within my my-pi-setups repository https://github.com/C3-TKO/my-pi-setups.


## Requirements

- Tested on Ansible 2.2.10
- Tested on Ubuntu 16.04 (xenial), but it should work on any modern Debian based system.

## Dependencies

This role expects that the host machine has already ufw and python setup - You can use my common role from the main repository to setup ufw and python 
https://github.com/C3-TKO/my-pi-setups/tree/master/ansible/roles/common

## Example playbook

You can include this role in your playbook like this:

    ---
    - name: Installs and configures redis
      hosts: redis
      become: yes
      become_method: sudo

    roles:
      - redis

## Licence

MIT

## Feedback? Found a bug? Requests?

Let me have it! https://github.com/C3-TKO/ansible-role-redis/issues
