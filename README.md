# Deploy webservers

Simple playbook to deploy apache, nginx include SELinux settings.
Nginx accepts https connections only 8443 port and translate it to apache 843 port.

# How to start

* Clone repository
* Fill ansible.cfg, add keys if nessesary
* Fill inventory file: hosts, add your host ip
* Run playbook via `$ ansible-playbook -i hosts deploy_apache_nginx.yml ` (add -vvv at the end if you need more diagnostic information)
* When playbook will finish, open address https://your-ip-address:8443 in your favourite browser.

# Goals
This code is written for educational purposes only.
