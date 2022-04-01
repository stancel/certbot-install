certbot-install
=========

Ansible role that downloads and installs the certbot / letsencrypt program to allow generation and renewal of "Let's Encrypt Authority" SSL certificates for website(s) that will be hosted on this same server.

Requirements
------------

None

Role Variables
--------------

None


Dependencies
------------

None

Example Playbook
----------------

Copy and edit *defaults/main.yml* to your *vars/main.yml*

```
	- hosts: your_server
	  vars_files:
	    - vars/main.yml
	  roles:
	    - stancel.certbot_install
```

License
-------

GPLv3

Author Information
------------------

[Brad Stancel](https://github.com/stancel) 