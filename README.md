# Splunk Deploy

Use Ansible to deploy Splunk Enterprise and Universal Forwarder on Linux

# Requirement

```bash
ansible-galaxy install -r requirements.yml -p ./
```

# Run

# Standalone Splunk Enterprise

```bash
ansible-playbook deploy-standalone.yml -i inventory.ini
```

# Universal Forwarder

# Distributed Splunk Enterprise

```bash
ansible-playbook deploy-distributed.yml -i inventory-distributed.ini
```
