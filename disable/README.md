Role Name
=========

Disable defined Network configurations. Which makes linux system hacker proof.

Requirements
------------
System Requirement: Centos7 , RHEL7 & above.

1) Ensure IP forwarding is disabled
2) Ensure packet redirect sending is disabled
3) Ensure IPv6 is disabled
4) Ensure DHCP is disabled
4) Ensure SCTP(stream control transoport protocol) is disabled
5) Ensure RDS is disabled
6) Ensure wireless interfaces are disabled


Role Variables
--------------

A description of the settable variables for this role should go here, variables that are in file/disablevars.yml.

- sysctl -w net.ipv4.ip_forward=0
- sysctl -w net.ipv4.conf.all.send_redirects=0
- sysctl -w net.ipv4.conf.default.send_redirects=0
- sysctl -w net.ipv6.conf.all.disable_ipv6=1
- sysctl -w net.ipv6.conf.default.disable_ipv6=1
- systemctl disable dhcpd

file/CISconfigfile.yml

- install rds /bin/true
- install tipc /bin/true
- install sctp /bin/true




Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: Centos
      roles:
         - disable


Author Information
------------------
Kamal Aggarwal 
Kartik Chopra   
