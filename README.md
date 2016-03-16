# cloud-init-utility
## Usage
``` bash
# ssh key stuff
ssh-agent bash
ssh-add cloud.key

# OpenStack client tool stuff
virtualenv env
source ./openstack.rc

# Launch VM with cloud-init configuration file
nova boot --image "ubuntu_cloud"  --key-name jing-key --flavor "m1.small" --availability-zone "node10" --user-data  your-cloud-config file your-vm-name --nic net-id=fc48a1d5-62e9-459f-89ab-86f4c0bf6486
```
## Delete VM
``` bash
nova delete your-vm-instance
```

## Todo
- DNS server ready
- puppet agent ready
- 
