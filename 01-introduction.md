# What is Ansible?

Ansible is an open-source automation tool used to manage multiple servers from one machine.

## Features

- Agentless (no software required on target servers)
- Uses SSH (Linux) and WinRM (Windows)
- Written in Python
- Uses YAML language
- Idempotent (same task repeated many times gives the same result)
- Push mechanism (Controller pushes tasks to nodes)

## Architecture

      Controller
  (Ansible Server)
         |
  ----------------
  |              |
Node1          Node2


- Controller = Machine where Ansible is installed.
- Managed Hosts = Servers controlled by Ansible.