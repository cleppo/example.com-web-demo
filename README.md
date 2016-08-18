EXAMPLE.COM WEBSITE DEMO 
========================

This project is intended to demonstrate my ability to administer a cloud configuration using multiple DevOps tools and disciplines.  It primarily utilizes Ansible roles and playbooks in conjunction with Travis CI to provide a reliable demo environment.

At the current time this project is not intended to represent any contribution to open source projects, just a way for me to demonstrate what I know and can do, as well as to learn new techniques and methods for creating a highly idempotent site configuration.


Requirements
------------



Role Variables
--------------


Dependencies
------------

NONE

Example Playbook
----------------

    - hosts: servers
      roles:
         - ec2-provisioning
         - { role: username.rolename, x: 42 }

License
-------

BSD
