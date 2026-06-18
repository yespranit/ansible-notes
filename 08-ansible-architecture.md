# Ansible Architecture

## Components

### Controller Node

The machine where Ansible is installed.

### Managed Nodes

Target servers controlled by Ansible.

### Inventory

Contains host information.

Default location:

```bash
/etc/ansible/hosts
```

### Modules

Small programs executed on managed nodes.

### Playbooks

YAML files used for automation.

## Architecture Diagram

```
            Controller
         (Ansible Server)
                 |
      ---------------------
      |                   |
    Node1               Node2
```

## Features

- Agentless
- Uses SSH
- Written in Python
- Uses YAML
- Idempotent
- Push-based architecture
```