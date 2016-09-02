EXAMPLE.COM-WEB ROLE
--------------------

Interview Project website-specific code/content.

Role to provide specific vhost configuration and content (index.html in this example) for the fictitious site www.example.com.  In the real world, the site content would usually be deployed via automated code release workflow/continuous integration.

The Jeff Geerling Apache role has a Jinja2 template for deploying the vhost config.  I will most likely rework this role to use it, however it appears that the Geerling role does not create directories or directly allow for vault encryption of files (like the SSL certificate and key files), so I created a role to handle that portion.  

I have seen instances where others have simply modified the Geerling role to fit their needs.  I decided to separate out my adaptations and changes for the sake of keeping the code clean and allowing for individual configuration of my vhosts.  I am open to suggestions that would work better, including arguments for simply modifying Geerling's role.


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

