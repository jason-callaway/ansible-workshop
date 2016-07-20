rhtps.vnc
=========

This role installs and configures TigerVNC on your RHEL or CentOS system.

rhtps philosophy
----------------

The rhtps Ansible roles were designed for a few specific use cases. Details [here](https://github.com/rhtps/philosophy).

Requirements
------------

None, however this is typically used in conjunction with the [rhtps.aws](https://github.com/rhtps/ansible-aws) role.

Role Variables
--------------

```vnc_username``` and ```vnc_password``` need to be set in the executing shell's environment.

Either export these, or edit ```env.sh``` and source it.

Dependencies
------------

* CDN: ```rhel-7-server-rpms```
* rhtps.yum role with above repo

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - rhtps.vnc

License
-------

Apache 2.0

Author Information
------------------

[Jason Callaway](https://github.com/jason-callaway) <jcallawa@redhat.com> is a Solutions Architect at Red Hat. 
