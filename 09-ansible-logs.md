# Ansible Logs

By default, Ansible does not create logs.

## Step 1: Open ansible.cfg

```bash
sudo vi /etc/ansible/ansible.cfg
```

Or:

```bash
vi ansible.cfg
```

## Step 2: Add log_path

Under [defaults]:

```ini
[defaults]
inventory = /etc/ansible/hosts
log_path = /var/log/ansible.log
```

## Step 3: Create Log File

```bash
sudo touch /var/log/ansible.log
sudo chmod 666 /var/log/ansible.log
```

Or:

```bash
sudo chown ansible:ansible /var/log/ansible.log
```

## Step 4: Run Playbook

```bash
ansible-playbook test.yml
```

## Step 5: Verify Logs

```bash
cat /var/log/ansible.log
```

Monitor in real time:

```bash
tail -f /var/log/ansible.log
```