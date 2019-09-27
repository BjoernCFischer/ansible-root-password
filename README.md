# ansible-root-password
Simple ansible role to set the root password

Requirements
------------

* A root password you want to set

Role Variables
--------------

*root_password* - the crypted root password to set, possibly stored in an ansible vault. For ways to create a crypted password see https://docs.ansible.com/ansible/latest/reference_appendices/faq.html#how-do-i-generate-encrypted-passwords-for-the-user-module

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-root-password, root_password: my_secret_crypted_root_password }

License
-------

Public domain.

Author Information
------------------

Björn Fischer - @BjoernCFischer
