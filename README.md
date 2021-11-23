Node Exporter
=========

[Node exporter source](https://github.com/prometheus/node_exporter)

Install Role
----------------

Add to requirements.yml

```
- name: node-exporter
  src: https://github.com/oleksandr-mazur/ansible-role-users
  version: master
```

```bash
$ ansible-galaxy install -r requirements.yml
```

Example Playbook
----------------

```yaml
- name: Setup node exporter
  hosts: my_hosts
  gather_facts: no
  roles:
    - role: node-exporter
      node_exporter_version: "1.3.0"
```

License
-------

BSD

