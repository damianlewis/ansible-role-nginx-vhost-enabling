# Ansible Role: Nginx vhost enabling
Uses Nginx's standard approach to enabling vhosts when using the [geerlingguy.nginx](https://galaxy.ansible.com/geerlingguy/nginx) role.

## Requirements
None.

## Role Variables
None.

## Dependencies
- geerlingguy.nginx

## Example Playbook
```yaml
- hosts: server
  become: yes

  tasks:
  - import_role:
      name: geerlingguy.nginx
  - import_role:
      name: damianlewis.nginx_vhost_enabling
```

## License
MIT

## Author
Damian Lewis