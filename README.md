common
=========

    Install packages and CA, enable and start services

Role Variables
--------------

    common_packages:    list of packages to be installed
    common_services:    list of services to be enabled and started
    common_ca:          path to root ca pem

Example Playbook
----------------

    - hosts: servers
      vars:
        common_epel: true
        common_packages: ['vim', 'tmux']
        common_services: ['haproxy']
        common_ca: '{{ role_path }}/certificates/ca.pem' 
      roles:
         - common

License
-------

    MIT

Author Information
------------------

    Dmitrij Petrov
