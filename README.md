common
=========

    Install packages, enable and start services

Role Variables
--------------

    common_packages:    list of packages to be installed
    common_services:    list of services to be enabled and started

Example Playbook
----------------

    - hosts: servers
      vars:
        common_packages: ['vim', 'tmux']
        common services: ['haproxy']
      roles:
         - { role: common }

License
-------

    MIT

Author Information
------------------

    Dmitrij Petrov
