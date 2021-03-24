OSP Instance delete
=========

Delete all Openstack instances defined.

Requirements
------------


Role Variables
--------------

Dependencies
------------

None

Example Playbook
----------------

    - hosts: workstation
      gather_facts: false
      become: yes
      vars:
        osp_cloud: openstack
        osp_servers:
          - instance_name: frontend
          - instance_name: app1
      roles:
        - name: osp-instance-delete

License
-------

BSD
