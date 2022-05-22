Role Name
=========

The Kafka role configures 3 aws EC2 instances as a kafka cluster.

Requirements
------------

Three EC2 instances with ubuntu .

Role Variables
--------------
kafka_binaries_url: The suitable kafka binaries url.
nodes: A list of the ansible_nodename of each ec2 instance
ips_blocks: Spcify the private ips of other instances and add 0.0.0.0 for the instance that has the file
ipsOfInstances: A list of the private ip of each instance.

Dependencies
------------
There is no Dependencies for this role.

Example Playbook
----------------

To be able to use this role, create a play book:
    - name: configure each node as a kafka broker
      hosts: servers
      gather_facts: true
      roles:
      - kafka-role

License
-------

BSD

Author Information
------------------
<a href="https://www.linkedin.com/in/abdurrhmansabry/">
<img src="https://www.vectorlogo.zone/logos/linkedin/linkedin-icon.svg" width="20" height="20"/> </a>