Role Name
=========

Deploy Vector system using ansible. Vector needs to collect, transform, and route logs, metrics, and traces.

Requirements
------------

Ansible >= 2.10 (It might work on previous versions, but we cannot guarantee it)

Role Variables
--------------
All variables which can be overridden are stored in defaults/main.yml file as well as in table below.

| Name | Default Value |	Description |
|------|---------------|--------------|
| `vector_version` | 0.52.0 | Vector package version. Also accepts latest as parameter. |
| `vector_arch` | x86_64 | Vector package architecture |
| `vector_sink_name` | clickhouse | Name of DB used |
| `vector_sink_type` | clickhouse | The type of sink |
| `vector_sink_address` | 127.0.0.1 | IP where is DB located |
| `vector_sink_table` | table1 | Name of table in DB |
| `ansible_user_id` | vector | Username to deploy role |
| `ansible_group_id:`| vector | User group for deploy role |
| `vector_source_name` | nginx | Source logs |
| `vector_source_type` | file | Source type |


Dependencies
------------

List of dependecies:
[Clickhouse role](https://github.com/AlexeySetevoi/ansible-clickhouse.git)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - vector-role

License
-------

MIT

Author Information
------------------

Leonid Fedin
