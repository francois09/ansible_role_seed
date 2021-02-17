Ansible Seed
============

Prepare ansible for newly provisionned server

Requirements
------------

N/A

Role Variables
--------------

N/A

Dependencies
------------

N/A

Example Playbook
----------------

When setting up a new machine, you can use:

```
- hosts: "{{ server_name }}"
  name: "Seed with ansible"
  become: yes
  gather_facts: False
  roles:
    # the following roles and tasks can be run in ansible :)
    - role: ansible_seed
```

License
-------

GPL v3

Author Information
------------------

François TOURDE
