#Provision and Configure OpenStack Instances in One Playbook Run

##tl;dr

```bash
curtis$ git clone https://github.com/curtisgithub/ansible-provision-openstack.git
curtis$ cd ansible-provision-openstack
curtis$ cp group_vars/openstack_instances.example group_vars/openstack_instances
curtis$ vi group_vars/openstack_instances # and edit with your openstack credentials
curtis$ vi roles/openstack_instances/tasks/main.yml # change set_fact line to be the correct name of private networks in openstack if necessary
curtis$ ansible-playbook -i nova.py site.yml
# done!
```

##Todo

* Pull groups from OpenStack metadata (like the official nova.py script does)
