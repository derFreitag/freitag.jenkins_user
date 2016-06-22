freitag.jenkins_user
===================
Ansible role to add and configure a system user for jenkins CI.

Requirements
------------
None

Role Variables
--------------
- ``jenkins_user_home`` defaults to ``/home/jenkins``, you may only change it for a jenkins master node to ``/var/lib/jenkins``.

**Optional variables**

*Please store them in ansible-vault or such!*

- ``ssh_public_key`` a public key to add to the user
- ``ssh_private_key`` a public key to add to the user
- ``authorized_keys`` list of SSH keys that should be allowed to login as jenkins user

Dependencies
------------
None

Example Playbook
----------------
Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: freitag.jenkins_user }

License
-------
GPLv3

Author Information
------------------
Gil Forcada Codinachs (der Freitag)