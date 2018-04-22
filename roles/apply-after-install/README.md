Synopsis
========

Apply this role right after a new host has been installed.


    $ ansible-playbook --limit <host> apply-after-install.yml --extra-vars "ansible_become_pass=<pass>"

The role provides:

* preinstall the following packages
* a password-less `sudo` (w/ resetting `HOME` environment variable)
