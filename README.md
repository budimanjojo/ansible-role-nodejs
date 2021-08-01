Ansible Packages Role
=====================

Role to install nodejs and npm from [NodeSource](https://github.com/nodesource/distributions).

Supported OS Families
---------------------

- Ubuntu (tested)
- Redhat (tested)

Role Variables
--------------

Available variables are listed below, the default values are in [defaults/main.yml](./defaults/main.yml):
```
nodejs_major_version: major version of nodejs you want to install, available versions can be found on [nodesource](https://github.com/nodesource/distributions), default to "16" (string)
```

Dependencies
------------

None

Example Playbook
----------------

Here is an example playbook:
```
- hosts: all

  vars:
    nodejs_major_version: "12"

  roles:
  - budimanjojo.packages
```

License
-------

MIT License
