EXAMPLE.COM-WEB ROLE

Interview Project website-specific code/content.

Role to provide specific vhost configuration and content (index.html in this example) for the fictitious site www.example.com.  

In the real world, the site content would usually be deployed via automated code release workflow/continuous integration.

Requirements
------------

Needs a role like geerlingguy-apache to install Apache and set up the base configuration.

Role Variables
--------------

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

