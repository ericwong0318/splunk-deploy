# Splunk Deploy

Use Ansible to deploy Splunk Enterprise and Universal Forwarder on Linux

# Requirement

Install the upstream vendor collection requirements locally before running the playbooks:

```bash
ansible-galaxy install -r requirements.yml -p ./
```

# Standalone Splunk Enterprise

```bash
ansible-playbook deploy-standalone.yml -i inventory.ini
```

# Universal Forwarder

# Distributed Splunk Enterprise

```bash
ansible-playbook deploy-distributed.yml -i inventory-distributed.ini
```

# Result

```bash
PLAY RECAP *********************************************************************************************************************************************************************************************************************
ericw-splunk-ansible-testing : ok=28   changed=0    unreachable=0    failed=0    skipped=22   rescued=0    ignored=0
ericw-uf3                  : ok=59   changed=15   unreachable=0    failed=0    skipped=55   rescued=0    ignored=0
```

# Health Check

![health_check](img/health_check.png)

![agent_management](img/agent_management.png)
