# UCLALib Ansible Role: Git [![Build Status](https://travis-ci.org/UCLALibrary/uclalib_role_git.svg?branch=master)](https://travis-ci.org/UCLALibrary/uclalib_role_git)

Installs the Git version control application using a pre-built rpm package install script.

## Requirements

Only supports RHEL-family servers at this time using the pre-built rpm package install script.

The install script name should use the format: `git-2.8.6.bin` where 2.8.6 is the bundled version of Git.

## Variables

* `git_version` - Defines the version of Git to be installed - this should match the version bundled in the packaged install script

## Dependencies

None.

## Example Playbook

```
---
    - name: uclalib_git_app.yml
      sudo: true
      hosts: servers

    roles:
      - { role: uclalib_role_git }
```

## License

BSD
