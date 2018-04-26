# Ansible Role: Elasticsearch

An Ansible Role that installs Elasticsearch on Debian.

## Requirements

- Requires at least Java 8+.
- Elasticsearch
- **2048mb minimum on ram**
- **2 CPU**
```
config.vm.provider "virtualbox" do |v|
  v.memory = 2048
  v.cpus = 2
end
```

## Dependencies

  - MarioDevment.elasticsearch

## Example Playbook

    #Java 1.8+ requiered
    #memory 2048mb or more and 2 cpu or more
    role: - MarioDevment.elasticsearch
    role: - MarioDevment.kibana

## License

MIT / BSD
