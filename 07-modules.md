# Ansible Modules

## What are Modules?

Modules are small programs used by Ansible to perform tasks on managed nodes.

## Common Modules

### Ping Module

```bash
ansible all -m ping
```

### Command Module

```bash
ansible all -m command -a "uptime"
```

### Yum Module

```bash
ansible all -m yum -a "name=httpd state=present"
```

### User Module

```bash
ansible all -m user -a "name=pranit state=present"
```

### Service Module

```bash
ansible all -m service -a "name=httpd state=started"
```

### Setup Module

```bash
ansible all -m setup
```

Collects facts about target servers.

## List All Modules

```bash
ansible-doc -l
```

## Module Documentation

```bash
ansible-doc yum
```