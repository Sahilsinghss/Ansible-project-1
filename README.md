# Ansible Role: Minikube

This role installs and configures Minikube on a single EC2 instance.

## Requirements

- Ansible >= 2.9
- Docker installed on the target machine

## Role Variables

| Variable            | Default Value | Description                   |
|---------------------|---------------|-------------------------------|
| `minikube_version`  | `latest`      | Minikube version to install   |
| `kubectl_version`   | `stable`      | kubectl version to install    |

## Example Playbook

```yaml
- name: Install Minikube
  hosts: all
  roles:
    - role: minikube
