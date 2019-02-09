Ansible role: refind
=========

[![MIT licensed][mit-badge]][mit-link]
[![Galaxy Role][role-badge]][galaxy-link]

Ansible role which installs and configures [rEFInd][refind-link].

Requirements
------------

NOTE: Role requires Fact Gathering by ansible!

The role Works with the following Systems:
 - MacOS

NOTE: The role requires the MacOS SIP (System Integrity Protection) to be turned off

Role Variables
--------------

| Variable | Description | Default |
|----------|-------------|---------|
| **refind_force_install** | If set to `yes` will overwrite the current rEFInd installation | `no` |

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: macbooks
  gather_facts: yes
  roles: drew-kun.refind
```

License
-------

[MIT][mit-link]

Author Information
------------------

Andrew Shagayev | [e-mail](mailto:drewshg@gmail.com)

[refind-link]: https://www.rodsbooks.com/refind/
[role-badge]: https://img.shields.io/badge/role-drew--kun.refind-green.svg
[galaxy-link]: https://galaxy.ansible.com/drew-kun/refind/
[mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
[mit-link]: https://raw.githubusercontent.com/drew-kun/ansible-refind/master/LICENSE
