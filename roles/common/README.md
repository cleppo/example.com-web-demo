COMMON ROLE
=========

This role is just a container for all the basic components I want every host in my environment to have.

TODO:  Get Travis CI tests working with meaningful success states.

Requirements
------------

No pre-reqs for this role since it is the basic setup for all hosts -- essentially STEP TWO after the ec2-provisioning step.

Role Variables
--------------


Dependencies
------------

NONE

Example Playbook
----------------

    - hosts: servers
      roles:
         - common
         - { role: username.rolename, x: 42 }

License
-------

BSD
