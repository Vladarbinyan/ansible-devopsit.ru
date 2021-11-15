Проект DEVOPSIT.RU
=========

Variables
--------------
Ключевые переменные перечислены в inventory/group_vars и inventory/host_vars

Dependencies
------------

Тестировалось и проверялось под ubuntu 20.04 lts. 

Playbooks
----------------



Play samples
------------

ansible-playbook play-deploy-ssh-keys.yml -u ubuntu --extra-vars "target=production" --ask-vault-pass  

ansible-playbook play-commontools.yml -u ubuntu --extra-vars "target=production" --ask-vault-pass  

ansible-playbook play-firewall.yml -u ubuntu --extra-vars "target=production" --ask-vault-pass  

ansible-playbook play-db.yml -u ubuntu --extra-vars "target=dbservers" --ask-vault-pass  

ansible-playbook play-webapp.yml -u ubuntu --extra-vars "target=appservers" --ask-vault-pass  

License
-------

MIT

Author Information
------------------

Командный проект ГБ. Вторая команда   
