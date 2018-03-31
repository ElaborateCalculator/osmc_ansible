# pitest
Using a VirtualBox VM with vagrant to simulate an osmc install on pi

## Vagrant
Bring up the VM with 
```vagrant up```
Requires the `debian/stretch64` box, version 9.4.0. SSH is set up on port
2322 by default, and the local directory is mounted at `/vagrant`

## Ansible
Execute the playbook with 
```ansible-playbook inittest.yml```
This performs the following tasks on the test VM:
1. Creates `osmc` user
1. Installs sudoers files
1. Adds ssh keys (hardcoded to my personal keys)
