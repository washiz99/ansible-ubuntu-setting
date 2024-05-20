# Ansible Ubuntu setup

Ansible roles to setup Ubuntu desktop.

## Requirement

Edit the sudoers file using visudo.

```bash
sudo visudo
```

Replace {user} with your username.

```text
# Allow members of group sudo to execute any command
%sudo   ALL=(ALL:ALL) ALL
{user}   ALL=NOPASSWD: /usr/bin/ansible-playbook
```

## Run playbook

```bash
ansible-playbook -i hosts site.yml
```
