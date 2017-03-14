UCLALib Ansible Role: Git [![Build Status](https://travis-ci.org/UCLALibrary/uclalib_role_git.svg?branch=master)](https://travis-ci.org/UCLALibrary/uclalib_role_git)
=========

Installs the Git version control application

Requirements
------------

Only supports RHEL-family servers at this time.

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

```
---
    - name: uclalib_git_app.yml
      sudo: true
      hosts: servers

    roles:
      - { role: uclalib_role_git }
      - { role: uclalib_role_git_app }

```

License
-------

BSD
