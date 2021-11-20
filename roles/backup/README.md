Роль backup
=========

Role Variables
--------------

Примеры приведены в defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------
play-backup.yml
---
- hosts: "{{ target }}"
  become: yes
  become_method: sudo
  roles:
    - {role: backup}

Play
------------

ansible-playbook play-backup.yml -u ubuntu --extra-vars "target=production"

License
-------

MIT

Author Information
------------------

