openstack-vm
============

Create an OpenStack VM from an existing image.

Requirements
------------

The controller (SDK) host requires the `openstacksdk` python module to communicate with the OpenStack instance.

The role assumes the `OS_*` environment variables have been set for OpenStack authentication.


Role Variables
--------------

See `defaults/main.yml`

Dependencies
------------

None.

Example Playbook
----------------

    - name: install a VM on an OpenStack cloud
      hosts: localhost
      roles:
      - role: openstack-vm
        openstack_vm_name: virtguest
        openstack_vm_image: cirros

License
-------

Apache-2.0 or MIT or BSD-3-Clause

Author Information
------------------

[James Cassell](https://github.com/jamescassell)
