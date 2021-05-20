# Execution

## Requirements

These playbooks leverage the Kubernetes Ansible collection. 
    https://docs.ansible.com/ansible/latest/collections/kubernetes/core/k8s_module.html#ansible-collections-kubernetes-core-k8s-module

Install with:
    `ansible-galaxy collection install kubernetes.core`

Additionally, the OpenShift python3 pip module:
    `sudo pip3 install openshift`

## Variables File

Review and update the [variables](./vars.yml) file as appropriate. 

The `ocp-cluster-name` variable is used in path lookup operations for the admin kubeconfig authentication.

These playbooks assume this repository has been cloned to your home directory, inside a cluster specific directory. e.g. `/home/pcunning-rh/cluster-1234/ocp4-console_branding`

Set values for install/remove logo/banner to "true" or "false" as features are desired.

## Install

`ansible-playbook -e "@vars.yml" install_console_customization.yml`

## Remove

`ansible-playbook -e "@vars.yml" remove_console_customization.yml`
