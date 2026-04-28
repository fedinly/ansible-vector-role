|Role Name
=========

Deploy Vector system using ansible. Vector needs to collect, transform, and route logs, metrics, and traces.

Requirements
------------

Ansible >= 2.10 (It might work on previous versions, but we cannot guarantee it)

Role Variables
--------------

| Name | Default Value |	Description |
| `vector_version` | 0.52.0 | Vector package version. Also accepts latest as parameter. |
| `vector_arch` | x86_64 | Vector package architecture |


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
