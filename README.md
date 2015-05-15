APT
==========

Install a list of packages. optionaly add PPA before

Requirements
------------

 - None

Role Variables
---------------

```yaml
---
apt:
  ppa:
    - ppa:ubuntu-lxc/lxd-git-master
  packages:
    - zsh
    - ubuntu-standard
    - emacs24-nox
```

Dependencies
------------

 - None

Example Playbook
----------------

```yaml
---
- hosts: webapp
  vars:
  roles:
    - role: apt
      apt:
        packages:
          - webapp
          - proxy
```

License
-------

MIT
