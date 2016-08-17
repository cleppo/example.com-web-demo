EC2 PROVISIONING ROLE
========================

This role is for provisioning EC2 instances to build my demo web site on.  This is the first role that is invoked to begin building the host(s) I need.

Requirements
------------

No pre-reqs for this role since it is the provisioning step for all hosts -- essentially STEP ONE

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
