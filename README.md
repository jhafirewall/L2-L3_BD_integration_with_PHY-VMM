# L2-L3_BD_integration_with_PHY-VMM

## Summary

This repository contains an ansible playbooks for automating Cisco ACI.
Ansible Playbook to Automate creation of EPG & BD and associate them to VMM or/and Physical Domain.

## Inventory & Variables

Update the variable of inventory.yaml & variables.csv based on your environment with APIC IP, credential and values in csv files.


## Instructions

These playbooks has been tested with Ansible 2.10 and Cisco ACI collection 2.0.0.

Cisco ACI ansible collection can be installed using the following command:

```
$ ansible-galaxy collection install cisco.aci
```

Cisco ACI ansible collection can be upgraded using either --force option or --upgrade option (available in 2.10+):

```
$ ansible-galaxy collection install cisco.aci --force
```

Before using these playbooks, ansible inventory and variable.csv needs to modified according to your environment.

To run the playbooks:

```
$ ansible-playbook FP.yaml -i inventory.yaml
```
