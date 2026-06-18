Inventory File Location
vi /etc/ansible/hosts
Example Inventory
[prod]
192.168.0.101

[dev]
192.168.0.102

[rhel6]
192.168.0.33
Verify Connectivity
ansible all -m ping

ansible prod -m ping

ansible rhel6 -m ping