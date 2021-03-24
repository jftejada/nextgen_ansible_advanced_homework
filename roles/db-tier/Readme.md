db Tier
=========

Ansible Role to:

- install postgress server
-

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


    - name: setup database tier
      hosts: apps
      become: yes
      gather_facts: false
      roles:
        - {name: base-config, tags: base-config}
        - {name: db-tier, tags: [apps, tomcat]}

License
-------

BSD
