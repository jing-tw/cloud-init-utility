# cloud-init-utility
## Usage
- virtualenv env
- source ./openstack.rc
- nova boot --image "ubuntu_cloud"  --key-name jing-key --flavor "m1.small" --availability-zone "node10" --user-data  your-cloud-config file your-vm-name --nic net-id=fc48a1d5-62e9-459f-89ab-86f4c0bf6486
