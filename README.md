# Ansible playbook to configure WordPress on Ubuntu

## Purpose 
wordpress-ansiblewordpress-ansible installs and configures WordPress on Ubuntu. Tested on Ubuntu 24.04.4 LTS

## Steps
1. Install Dependencies
2. Install WordPress
3. Configure Apache for WordPress
4. Configure database
5. Configure WordPress to connect to the database

## How to use it
1. On a management server clone the repository
2. Update the public IP of the server in inventory.ini
3. Run ansible playbook: ansible-playbook -i inventory.ini site.yml --extra-vars "db_pass=<your-db-password> ansible_sudo_pass=<your-sudo-password>"
4. Proceed with WordPress configuration on WordPress UI

