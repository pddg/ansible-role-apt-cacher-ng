apt-cacher-ng
=========

Role for installing and configuring apt-cacher-ng and setup its client.

Requirements
------------

You should have `sudo` permission. 

Role Variables
--------------

See [defaults/main.yml](./defaults/main.yml)

Dependencies
------------

No dependencies

Example Playbook
----------------

```yaml
---
- hosts: all
  become: yes
  roles:
    # Server and client
    - name: pddg.apt_cacher_ng
      vars:
        apt_cacher_server: yes
    # Client only
    - name: pddg.apt_cacher_ng
      vars:
        apt_cacher_server: no
```

License
-------

MIT

Author Information
------------------

[pddg](https://github.com/pddg/)
  - Web: [poyo.info](https://www.poyo.info/)

