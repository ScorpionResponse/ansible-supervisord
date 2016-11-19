Ansible Role: Supervisord
=========================

[![Build Status](https://travis-ci.org/ScorpionResponse/ansible-supervisord.svg?branch=master)](https://travis-ci.org/ScorpionResponse/ansible-supervisord)

Ansible role to install supervisord.

Requirements
------------

None.

Role Variables
--------------

* `supervisord_user_name`: The user acccount name to run supervisord under.
  Default: supervisord
* `supervisord_grop_name`: The group name to run supervisord under.  Default:
  supervisord
* `supervisord_config_dir`: The directory to install configuration files into.
  Default: /etc/supervisord
* `supervisord_log_dir`: The directory to store all of the logs.  Default:
  /var/log/supervisord

Dependencies
------------

* Will use ScorpionResponse.pip role to install pip.

Example Playbook
----------------

Example usage:

    - hosts: all
      roles:
         - { role: ScorpionResponse.supervisord }

License
-------

BSD

Author Information
------------------

Github: https://github.com/ScorpionResponse
