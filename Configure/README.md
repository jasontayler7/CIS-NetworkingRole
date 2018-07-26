Role Name
=========

This role configure defined Network configuration.

Requirements
------------

System Requirement: RHEL7 /Centos7 & above.

TASKS
------------

- Ensure TCP Wrappers is installed
- Ensure /etc/hosts.allow is configured
- Ensure /etc/hosts.deny is configured
- Ensure permissions on /etc/hosts.allow are configured
- Ensure permissions on /etc/hosts.deny are configured
- Ensure iptables is installed
- Ensure default deny firewall policy
- Ensure loopback traffic is configured
- Ensure outbound and established connections are configured
- Ensure firewall rules exist for all open ports

Role Variables
--------------
In this we used variable and stored in the files folder ( protocol, port, ipaddress & outbound)

Dependencies
------------
No dependencies and any other role required.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

Author Information
------------------

Kamal Aggarwal

Kartik Chopra
