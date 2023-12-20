Role Name
=========

Install and setup kibana 

Requirements
------------


Role Variables
--------------

---

kibana_version: version of kibana

elasticsearch_ca_name: elasticsearch-ca.pem same name of the setting in elasticsearch

### SSL 
ssl_enabled: enable yes or no
certificate_ssl_name: kibana-server
dns_enable: enable yes or no
dns_name: name of dns

### Settings
kibana_https_enabled: if kibana https xpack is enabled

kibana_old_space_mb: size of kibana old space mb, use 1024 such as default 

kibana_install_mode: https 

elasticsearch_security_enabled: if elasticsearch xpack is enabled

elasticsearch_https_enabled: if elasticsearch https is enabled

elasticsearch_username: kibana_system username

elasticsearch_password: password used in elasticsearch config

path_elastic: elasticsearch path

elastic_stack_ca: same file of elasticsearch

elastic_stack_ca_password: password used in elasticsearch config

Dependencies
------------

 

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: kibana
  become: true
  roles: 
    - ../roles/kibana

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
