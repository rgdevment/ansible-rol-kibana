# URL ROL

https://galaxy.ansible.com/MarioDevment/kibana/

# Ansible Role: Kibana

An Ansible Role that installs Kibana on Debian.

## Requirements

- Requires at least Java 8.
- Elasticsearch
- **Memory: 2048mb minimum**
- **2 CPU**

```
config.vm.provider "virtualbox" do |v|
  v.memory = 2048
  v.cpus = 2
end
```

## Role Variables

    server_host: 0.0.0.0
    server_name: debianserver
    server_elastic_search: 0.0.0.0

## Dependencies

  - MarioDevment.elasticsearch

## Example Playbook

    role: - MarioDevment.elasticsearch
    role: - MarioDevment.kibana

## License

MIT / BSD
