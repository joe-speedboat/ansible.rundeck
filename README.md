# Ansible Rundeck Role
This is a role to install Rundeck with Nginx ssl reverse proxy and mariadb on single host

## Ansible env
* Ansible: 11.1.0

## Tested OS
- Rocky Linux 9

## Role Variables
Variables are documented or self speaking by its names.   
Look into defaults folder to get an overview of your needs.   
It is strongly recomended to change sensitive variables such as passwords.   

The role can install a local Ansible control-node runtime for Rundeck by using
`joe-speedboat/ansible.installer`. This is enabled by default with:

```yaml
rundeck_install_ansible: true
rundeck_ansible_installer_url: https://raw.githubusercontent.com/joe-speedboat/ansible.installer/refs/heads/main/ansible/ansible_setup.sh
rundeck_ansible_installer_path: /usr/local/sbin/ansible_setup.sh
rundeck_ansible_uv_marker: /opt/ansible/.ansible-uv-installer
```

Set `rundeck_install_ansible: false` if Ansible is managed by another control-node
runtime on the same host.

## How to use
`ansible-playbook tests/install_rundeck.yml`

## Dependencies
* `ansible-galaxy role install -r roles/requirements.yml`

## License
https://opensource.org/licenses/LGPL-3.0    
Copyright (c) Chris Ruettimann <chris@bitbull.ch>  

