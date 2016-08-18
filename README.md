EXAMPLE.COM WEBSITE DEMO 
========================

This project is intended to demonstrate my ability to administer a cloud configuration using multiple DevOps tools and disciplines.  It primarily utilizes Ansible roles and playbooks in conjunction with Travis CI to provide a reliable demo environment.

At the current time this project is not intended to represent any contribution to open source projects.  It's just a way for me to demonstrate what I know and can do, as well as to learn new techniques and methods for creating a highly idempotent site configuration.


Requirements
------------

Dependencies
------------

I've used the Apache role created by Jeff Geerling with no changes.  The goal is to use the role and add my unique configuration on a site-by-site basis.

Notes
-----

You will notice that I've installed the Puppetlabs repo and git on these hosts.  The goal here is to use ansible to stand up my enviroment and test using Puppet to manage my configuration as well.  My initial foray into creating playbooks is under the playbooks/puppetserver directory.  I created a giant playbook that ends up building a puppet master.  My ultimate goal will be to create an ansible puppet master role (WHY??? Just 'cause I can.   :D   ).

TODO:  It is likely that the standitup.yml playbook will end up being my site.yml playbook.  I would like to have the provisioning role create a set number of hosts with a predetermined prefix (like "web" for webservers) followed by a meaningful number (like the last two octets of the RFC 1918 IP address).

License
-------

BSD
