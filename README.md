# vnf-lcm-bootstrapping
Ansible roles to bootstrap VNF LCM Server

## Dependencies
The requirements to run this script are:

Openstack Client VM with all required bundles installed (See Openstack client VM in Rackspace cloud), and Root access.
Ansible 2.9.1 or higher\
Git\
PIP Packages\
python-openstacksdk==0.5.2
python-cinderclient==5.0.0
python-heatclient==1.18.0
python-keystoneclient==3.21.0
python-openstackclient==3.19.0
python-openstacksdk==0.5.2
pexpect==4.7.0\
Access to the OpenStack API as ADMIN

## Pre-requisites
Ensure that below pre-requisites are completed before executing the Ansible playbook.

1. Login to the client VM as root and source the admin keystone file.

2. Ensure that the External Network, Subnet and associated resources are created for the Tenant


## Playbook Execution
1. Navigate to below directory and edit the vars file with the required parameters.

2. Once the var files are updated, navigate to the parent folder for the source code and execute below command\
ansible-playbook boostrap.yml