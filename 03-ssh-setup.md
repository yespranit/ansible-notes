# SSH Configuration

## Configure Hostname

```bash
hostnamectl set-hostname ansible.radical.com
```

## Edit Hosts File

```bash
vi /etc/hosts
```

Add:

```text
192.168.0.100 ansible.radical.com
192.168.0.101 node1
192.168.0.102 node2
```

## Generate SSH Key

```bash
ssh-keygen
```

Press Enter three times.

Keys are stored in:

```text
/root/.ssh/
```

Check:

```bash
ls /root/.ssh
```

Output:

```text
id_rsa
id_rsa.pub
```

## Copy Key to Node1

```bash
ssh-copy-id root@192.168.0.101
```

## Copy Key to Node2

```bash
ssh-copy-id root@192.168.0.102
```

## Verify Passwordless SSH

```bash
ssh root@192.168.0.101
ssh root@192.168.0.102
```

No password should be asked.