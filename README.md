certbot-install
=========

Ansible role that downloads and installs the certbot / letsencrypt program to allow generation and renewal of "Let's Encrypt Authority" SSL certificates for website(s) that will be hosted on this same server.

Requirements
------------

None

Role Variables
--------------

URL of where to download the certbot binary. The default is 'https://dl.eff.org/certbot-auto'.
```
	certbot_install_url: "https://dl.eff.org/certbot-auto"
```

Directory on target server to store the certbot binary. The default is '/opt/certbot'.
```
	certbot_install_dir: "/opt/certbot"
```

Dependencies
------------

None

Example Playbook
----------------

Copy and edit *defaults/main.yml* to your *vars/main.yml*

	- hosts: your_server
	  vars_files:
	    - vars/main.yml
	  roles:
	    - stancel.certbot_install


or just pass the variables in the playbook


	- hosts: your_server 
	  vars:
		certbot_install_url: "https://dl.eff.org/certbot-auto"
		certbot_install_dir: "/opt/certbot"
	  roles:
	    - stancel.certbot_install

License
-------

GPLv3

Author Information
------------------

[Brad Stancel](https://github.com/stancel) 


