atom-packages
=============

Ansible role for installing pacakges for the Atom editor

Requirements
------------

Install the Ansible, the Atom and the apm (Atom Package Manager) command.

Role Variables
--------------

- atom_packages_packages
    - an array of atom packages

Dependencies
------------

None.

Example Playbook
-------------------------

    - hosts: localhost
      connection: local
      gather_facts: no           
      sudo: no
      vars:
        atom_packages_packages:
          - project-manager
          - recent-files
      roles:
        - hnakamur.atom-packages

License
-------

MIT

Author Information
------------------

Hiroaki Nakamura's contact information is at https://hnakamur.github.io/
