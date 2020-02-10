## Create mariadb docker instance

The main requirements are:
1. Install a centos 7 vm.
2. Install docker on this vm.
3. Install mariadb docker image.


### Step 1 installing a vm on GCP

This example is taken from the Ansible GCP guide

https://docs.ansible.com/ansible/latest/scenario_guides/guide_gce.html
Some extra plugins need to be installed with the following command.

`pip install requests google-auth python-requests`

A service-account needs to be created and saved in a secure location

### Step 2

Next step is linked in the main playbook installing the latest docker version on the vm.

### Step 3

The final step is to install the database server.

### Executing the playbook

`ansible-playbook --ask-vault-pass create_vm.yml`

password supersecretpassword
