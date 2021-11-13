Роль commontools
=========

Role Variables
--------------

Dependencies
------------

None

Example Playbook
----------------
play-commontools.yml
---
- hosts: "{{ target }}"
  become: yes
  become_method: sudo
  roles:
    - {role: commontools}

Play
------------

ansible-playbook play-commontools.yml -u ubuntu --extra-vars "target=production"

License
-------

MIT

Author Information
------------------

https://github.com/Vladarbinyan/