# Ansible playbook

Prerequisites:

- Debian 10 minimal installation
- with ssh server (you may want to enable password authentication)

After minimal installation Debian 10 just run this playbook.

```bash
apt install -y ansible
ansible-playbook main.yml
```

To enable login to ssh with passwords, run with:

```bash
ansible-playbook main.yml --extra-vars 'sshkeysonly=false'
```

And reboot the machine.
