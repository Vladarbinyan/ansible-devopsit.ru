Роль manage-firewall
=========

Role Variables
--------------

Dependencies
------------

None

Example Playbook
----------------
play-firewall.yml
---
- hosts: "{{ target }}"
  become: yes
  become_method: sudo
  roles:
    - {role: manage-firewall}

Play
------------

ansible-playbook play-firewall.yml -u ubuntu --extra-vars "target=production"

License
-------

MIT

Author Information
------------------

https://github.com/Vladarbinyan/