# Ad Hoc Commands

## Ping All Hosts

```bash
ansible all -m ping
```

## Check Uptime

```bash
ansible all -m command -a "uptime"
```

## Mount Information

```bash
ansible all -m command -a "mount"
```

## Install HTTPD Package

```bash
ansible all -m yum -a "name=httpd state=present"
```

## Verify User

```bash
ansible all -m command -a "id pranit"
```

## Create User

```bash
ansible all -m user -a "name=pranit state=present"
```

## Reboot Servers

```bash
ansible all -m command -a "reboot"
```

## Collect System Information

```bash
ansible all -m setup
```

The setup module gathers facts about all servers.