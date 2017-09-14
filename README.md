[![Build Status](https://travis-ci.org/teadur/ansible-observium-agent.svg?branch=master)](https://travis-ci.org/teadur/ansible-observium-agent)

observium-agent
=========

This role manages observium-agent on Linux.
It configures install/configures xinetd to run obserivum-agent and deploys defined agent plugins to host.


Requirements
------------

Xinetd running on host ( installed by this role )

SNMP running on host ( only configuration is modified, one oid is added, must be installed by some other role) 

Role Variables
--------------

observium_host: host running observium ( defaults to 127.0.0.1 )
 
obs_agent_pg_enable: boolean (default false)

obs_agent_apache_enable: boolean (default false)

obs_agent_bind_enable: boolean (default false)

All variables can be found in defaults/main.yml


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: teadur.observium-agent }

License
-------

MIT

Author Information
------------------

Georg Kahest georg[at]gj.ee
