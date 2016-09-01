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

You may notice that I've included the Puppetlabs repo and git in the code.  My intent here is to use ansible to stand up my enviroment and test using Puppet to manage my configuration as well.  FYI - my initial foray into creating playbooks is under the playbooks/puppetserver directory (playbooks/puppetmaster/gimme_puppet.yml.2.0).  I created a giant playbook that ends up building a puppet master.  It's not very elegant and more of a laundry-list script instead of good playbook code, but it works.  If I ever get time I may play around with it and see if I can turn it into a respectable role and submit it to Ansible Galaxy.  (WHY??? Just 'cause I can.   :D   ).

TODO:  It is likely that the standitup.yml playbook will end up being my site.yml playbook.  I would like to have the provisioning role create a set number of hosts and either create or destroy them as needed at playbook runtime by specifying a count value at playbook runtime.

 TODO:  the SSH wait step currently hangs when hosts are being terminated.  I need to set this task to skip when the count value specified at runtime is equal to or greater than the existing number of nodes.

TODO:  Get Travis CI tests working with meaningful success states.

TODO - Make ssh fingerprint step clean up duplicate entries (from multiple runs creating the same host)

TODO:  FIX certificate tags (and the contents in the vault file) so that multiple certs can exist in the same vault.

TODO:  Variablize the cert and key filenames for better idempotency.

References:
-------

Since this is a work-in-progress, for learning/demonstration purposes I do not yet have a reliable set of references/sources for the code shown here.  Once I get everything working at a satisfactory level, I will credit my sources as best I can.

So far I will say that Jeff Geerling's work has been a great influence in my learning so far and I will reference his source material in this section when I am able to.

License
-------

BSD


