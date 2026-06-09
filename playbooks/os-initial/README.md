# os-initial playbook

Before using this role for the first time, complete the following steps.

## 1. Create the Configuration File

Copy `group_vars/default.all.yml` to `group_vars/all.yml` and modify it according to your requirements:

```bash
cp group_vars/default.all.yml group_vars/all.yml
```

## 2. Create the Inventory File

Copy `default.hosts` to `hosts` and update it with your host information:

```bash
cp default.hosts hosts
```

## 3. Run the Initialization Playbook

After completing the configuration, run the initialization playbook.

```bash
ansible-playbook -i hosts os-initial.yml
```
