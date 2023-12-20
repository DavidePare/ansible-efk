Role Name
=========

Role to deploy the honeypot Cowrie

Requirements
------------

Tested on Ubuntu 20 

Role Variables
--------------

cowrie_user: cowrie # IMPORTANT: Don t change it. 

github_cowrie: http://github.com/cowrie/cowrie # link to download the honeypot

name_virtualenv: name of the environment

path_to_virtualenv: virtual-environment path

new_ssh_port: port to move the real ssh port 

cowrie_ssh: true or false if you are monitoring the ssh port

cowrie_telnet: true or false if you are monitoring the telnet port

Dependencies
------------

No dependencies only need virual-environment

Example Playbook
----------------

- hosts: monitoring
  become: true
  roles: 
    - ../roles/cowrie

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
