# Ansible Multiple WordPress

Provisions an Ubuntu server to run multiple WordPress sites with Ansible.

This won't set up an entirely new wordpress site, it is meant for migrating existing WordPress sites to a single server.

You will need to store your wordpress sites in separate git repositories and manually migrate your databases.

The provision playbook will set up nginx, php5-fpm, and mysql.

The deploy playbook will pull the latest code for each site and restart php5-fpm.

Files you will need to modify for your site/server settings

* group_vars/all
* hosts
