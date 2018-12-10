[![Build Status](https://www.travis-ci.org/securCom/ansible-role_repo-scl.svg?branch=master)](https://www.travis-ci.org/securCom/ansible-role_repo-scl)
[![GitHub release](https://img.shields.io/github/release/securCom/ansible-role_repo-scl.svg)](https://github.com/securCom/ansible-role_repo-scl)


# Repo: SCL

Manage  Software Collections ( SCL ) Repository

# Requirements

For supported systems  see https://wiki.centos.org/AdditionalResources/Repositories/SCL. If your system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `scl_repo_package_state`: the epel package presence  state

# Dependencies

There no external dependencies.

# Example Playbook

To install role, add following line to **ansible-galaxy** requirements file
```
- src: https://github.com/securCom/ansible-role_repo-scl
  version: master
  name: securcom.repo_scl
```

```
- hosts: servers
  roles:
     - securcom.repo_scl
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)