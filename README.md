Role Name
=========

This role installs the Bamboo elastic agent.

https://confluence.atlassian.com/bamboo/creating-a-custom-elastic-image-linux-296093037.html

Requirements
------------

You need to install a JRE (or JDK) on your instance to be able to run the agent. 

https://confluence.atlassian.com/bamboo/supported-platforms-289276764.html#Supportedplatforms-Java.1

Role Variables
--------------

bamboo_elastic_agent_url: Currently set to the URL for version 4.1; override if you want a different version.

Example Playbook
----------------

    - hosts: bamboo_elastic_agent
      gather_facts: true
      sudo: true
      roles:
        - bamboo-elastic-agent

License
-------

MIT
