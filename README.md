# About
This ansible playbook is used to deploy a simple uwsgi web app.

# Requirements
Target system must be debian or downstream derivatives. A registered domain name, SSL certificate, and email server are
required. If using a subdomain, a CNAME entry must be commited to the appropriate DNS record.

# Usage
Ensure that the `group_vars/all` and `hosts` files are correctly configured. To execute the playbook, issue the following command:

```bash
ansible-playbook --inventory=hosts -vv --private-key=~/.ssh/private_key --ask-become-pass deploy.yml
```
