LB Tier
=========

Ansible Role to:

- install haproxy to load balance traffic


Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

Example usage:


    - name: setup load balancer tier
      hosts: apps
      become: yes
      gather_facts: false
      roles:
        - {name: base-config, tags: base-config}
        - {name: lb-tier, tags: [lbs, haproxy]}

License
-------

BSD
