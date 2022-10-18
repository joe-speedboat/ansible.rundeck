# Ansible Rundeck Role
This is a role to install Rundeck with Nginx ssl reverse proxy and mariadb on single host

## Ansible env
* Ansible Core: 2.13

## Tested OS
- Alma Linux 8
- Alma Linux 9

## Role Variables
Variables are documented or self speaking by its names.   
Look into defaults folder to get an overview of your needs.   
It is strongly recomended to change sensitive variables such as passwords.   

## How to use
`ansible-playbook tests/install_rundeck.yml`

## Dependencies
* `ansible-galaxy role install -r roles/requirements.yml`

## License
https://opensource.org/licenses/LGPL-3.0    
Copyright (c) Chris Ruettimann <chris@bitbull.ch>  

