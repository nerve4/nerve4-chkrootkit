# CHkrootkit

An Ansible role that installs chkrootkit to CENTOS 8, Rocky9 and Ubuntu. More info about CHkrootkit: [link](http://www.chkrootkit.org/)


## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

## Tasks descriptions

- main.yml - Run the OS check and run the relevant playbook
- install_el8.yml - Deploy chkrootkit on Rhel8.x
- install_ubuntu.yml - Deploy chkrootkit on Ubuntu


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-chkrootkit
```

## Maintainer Information
Lee | 2023