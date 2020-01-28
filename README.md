User Management
=========

Create or delete user

Requirements
------------

No specific required Ansible

Role Variables
--------------

#Define the user name
user_name:
user_state: present

Dependencies
------------

None

Example Playbook
----------------

---
- hosts: all
  connection: paramiko
  tasks:
    - include_role:
        name: user_mgt
      vars:
       user_name: test
       user_state: absent

License
-------

MIT

Author Information
------------------

muhannadengineer@gamil.com
