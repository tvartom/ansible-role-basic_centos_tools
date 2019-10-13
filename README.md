ansible-role-basic_centos_tools
===============================

Some basic setup for CentOS 7 as an Ansible-role.

Requirements
------------

CentOS 7

Role Variables
--------------

basic.timezone
basic.package_to_install

Look at defaults in defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      tasks:
         - include_role:
             name: ansible-role-basic_centos_tools
           vars:
             basic:
               timezone: "Europe/Stockholm"
               package_to_install:
                 - mc
                 - rsync

License
-------

CC-BY-4.0

Author Information
------------------

tvartom

