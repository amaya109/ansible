# os-initial playbook

Before using this role for the first time, complete the following steps.

## 1. Install the collections required for Ansible playbook.

```bash
ansible-galaxy collection install -r requirements.yml
```

## 2. Create the Inventory File

Copy `default.hosts` to `hosts` and update it with your host information:

```bash
cp default.hosts hosts
```

## 3. Run the Prometheus Playbooks

After completing the configuration, run the prometheus playbooks.

```bash
# example:
ansible-playbook -i hosts prometheus.yml
ansible-playbook -i hosts alertmanager.yml
```
