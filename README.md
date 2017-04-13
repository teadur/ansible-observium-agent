observium-agent
=========

This role manages observium-agent on Debian based Linux.
It configures xinetd to run obserivum-agent and deploys defined agent plugins to host.

Requirements
------------

Xinetd running on host ( installed by this role )
Role Variables
--------------

observium_host: host running observium ( defaults to 127.0.0.1 ) 
obs_agent_pg_enable: boolean (default false)
obs_agent_apache_enable: boolean (default false)
obs_agent_bind_enable: boolean (default false)

All variables can be found in defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: observium-agent }

License
-------

MIT

Author Information
------------------

Georg Kahest georg[at]gj.ee
