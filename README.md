Ansible Role: PHP
=========

This role installs the latest versions of php (via Sury) and also allows you to configure :

- php-fpm config
- php-fpm default pool (dynamic and ondemand modes)
- opcache
- php.ini
- apcu

Requirements
------------

Nginx must be installed beforehand.

Role Variables
--------------

By default, the version of php installed will be php 7.4. This can be changed
by changing the following variable:

    php_version: 7.x

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: julien_langlois.php, x: 42 }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2020 by [Julien Langlois](https://github.com/julien-langlois).
