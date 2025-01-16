Role Name
=========

This Ansible Role is used to install and configure all the prereqs required for running a LEAPP upgrade.

Requirements
------------

This Role is only designed to be used on Red Hat Enterprise Linux 7,8 and 9. LEAPP is a tool used to complete inplace upgrades for RHEL.The only requirements are to have your RHEL system subscribed to either Red Hat Satellite Server or to the Red Hat Content Delivery network.

Role Variables
--------------

The variables used in this role are as follows.

# Used to set the version of RHEL that will be upgraded from. This is to ensure the correct repositories are enabled.
## leapp-prereqs-rhel-ver: 7

Dependencies
------------

None

Example Playbook
----------------

To include the role in your playbooks you can use similar to below.

    - hosts: servers
      roles:
         - { role: ansible-role-leapp-prereqs }

License
-------

BSD

Author Information
------------------

Role has been developed by Ken Hitchcock
github.com/kenhitchcock
