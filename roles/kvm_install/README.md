KVM_Install
=========

Installs KVM and Cockpit

Example Playbook
----------------

- name: Setup KVM on Bare Metal

  hosts: bare_metal

  become: yes

  roles:

    - role: kvm_install

License
-------

BSD

