**debian_updates**
==============

An Ansible role to upgrade Debian packages and automatically reboot the system when required.

Requirements
------------

- Debian.
- Ansible Core 2.18 or newer.
- Privileged access to the managed host.
- Network access to configured APT repositories.
- Python and the dependencies required by `ansible.builtin.apt` on the managed host.

Role Variables
--------------

No configurable role variables are currently defined.

Dependencies
------------

No additional Ansible roles are required.

Example Playbook
----------------

```yaml
---
- name: Update Debian servers
  hosts: debian
  become: true

  roles:
    - debian_updates
```

License
-------

MIT

Author Information
------------------

TheWolfPaws