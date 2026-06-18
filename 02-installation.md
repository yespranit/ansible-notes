# Ansible Installation

## Verify Connectivity

```bash
ping 192.168.0.101
ping 192.168.0.102
```

Both nodes should reply.

## Install Ansible

### RHEL 8/9

```bash
yum search ansible
yum install ansible -y
```

## Verify Installation

```bash
ansible --version
```

## Verify Python

Controller:

```bash
python3 --version
```

Node1:

```bash
python3 --version
```