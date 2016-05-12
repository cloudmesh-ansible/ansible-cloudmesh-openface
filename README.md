Cloudesh Ansible Openface
=========================

This role is not yet operational.

Requirements
------------

* Account on a cloud
* cloudmesh instalation in case of automated booting

Role Variables
--------------

* cloud: the name of the cloud as specified in the yml file.

* number: the number of the vms (1-3)

Dependencies
------------

None

Example Playbook
----------------

Deploy cloudmesh

    ansible-playbook tasks/cloudmesh.yml

Start a number of virtual machines with cloudmesh on cloud cm

    ansible-playbook tasks/boot.yml -e count=2

List the inventory

    cat inventory.txt

For each ip do

    rm ~/.ssh/known_hosts
    ssh cc@<IP> uname

Stat the deployment

    ansible-playbook  tasks/main.yml -i inventory.txt -u cc


License
-------

Apache 2.0

Author Information
------------------

Gregor von Laszewski (laszewski@gmail.com)

