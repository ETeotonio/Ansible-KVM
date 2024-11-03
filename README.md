# Ansible-KVM

Playbook and Role to Install KVM and Cockpit to Rocky Linux 9.

## Pre-requirements

- Rocky Linux 9 - https://rockylinux.org/download

    - Additional Packages installed:
        
        - sshpass

        - openssh


- Ansible Core 2.15.12 - install using ```pip3 install ansible-core```

## Folder Organization

── inventory - containing the inventory.yml with the hosts

├── playbooks - with the Playbook invoking the role

└── roles - with the roles

    └── kvm_install

        ├── meta

        └── tasks - Tasks to install KVM and Cockpit

## How to Run the Playbook

Use the following command to test:

```ansible-playbook playbooks/kvm.yml --check``

Use the following command to run the playbook:

```ansible-playbook playbooks/kvm.yml -kK``