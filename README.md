Ansible Salt
=========

1. install minion on all nodes (or in a specified group)
2. install master on all nodes in master group
3. configure master host on all minions
4. configure master
5. generate keys for all minions
6. preseed minions with accepted keys
8. start master
9. start minions

Requirements
------------

Minion nodes must be able to resolve master node.

See example in tests/test.yml

License
-------

GPL 3.0

Testing
-----

```shell
cd tests
vagrant up
ansible-playbook -b  test.yml -i .vagrant/provisioners/ansible/inventory/vagrant_ansible_inventory