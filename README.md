# Ansible Rundeck Role
This is a role to install Rundeck with Nginx ssl reverse proxy and mariadb on single host

## Execution Requirements
- Tested with CentOS7

## Role Variables

### The following variables may be overridden:
* `rundeck_domain`: fqdn that get accessed by web browser
* `rundeck_admin_pass`: rundeck web admin password
* `mariadb_root_password`: MariaDB root password
* `mariadb_user_password`: rundeck DB user password

## How to use
`ansible-playbook tests/install_rundeck.yml`

## Dependencies
* `role`: joe-speedboat.mariadb 

## License
https://opensource.org/licenses/LGPL-3.0    
Copyright (c) Chris Ruettimann <chris@bitbull.ch>  

