Role Name
=========

This role installs nginx under Debian 10 / Ubuntu 18.04, 20.04 and RHEL / CentOS 8.
The default config will be found under templates/nginx.conf.j2 and enables the Debian default directory Structure under RHEL / CentOS, too.
Place your vHosts in /etc/nginx/sites-available and link them into /etc/nginx/sites-enabled.

The default vHost will be enabled, for better Let's Encrypt certbot compatibility out of the box.

Requirements
------------

Ansible >= 2.9

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: nginx
      roles:
         - { role: kornkalle.ansible_nginx }

License
-------

GPLv3

Author Information
------------------

n.berg@backslashseven.de
