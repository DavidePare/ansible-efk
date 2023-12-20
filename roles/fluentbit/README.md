Role Name
=========

Install and configure fluentbit

Requirements
------------


Role Variables
--------------

fluentbit_path_conf: path fluentbit

path_log: path where retrieve the logs

fluentd_port: port to send the log

type_parsing: format such as json

Dependencies
------------



Example Playbook
----------------

- hosts: monitoring
  become: true
  roles: 
    - ../roles/fluentbit

License
-------

BSD

Author Information
------------------

