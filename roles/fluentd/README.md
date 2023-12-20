Role Name
=========

Install and configure fluentd

Requirements
------------


Role Variables
--------------

---
# defaults file for fluentd

reserved_port: port reserved to fluentd

elastic_virtual_proto: if https enabled

logstash_format: if the logs will be send using the logstash format
elasticsearch_port: elasitsearch port to send data

elasticsearch_fluentd_account_user: fluentd user to send data to elasticsearch node
elasticsearch_fluentd_account_password: fluentd passwotd to send data to elasticsearch node



fluentd_config_path: where fluentd will be installed

listen_port: where fluentd will receive the logs

elasticsearch_https_enabled: if https enabled

use_ipv6: if you want to use ipv6 (boolean)




Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: fluentd
  become: true
  gather_facts: true
  roles: 
    - ../roles/fluentd

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
