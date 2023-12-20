Deploy EFK with Ansible

# Requirements
The machine which will lunch they playbooks need: python3 and ansible installed. 
All the other machines need python3.

# Start
Modify the file hosts.ini  and change the password inside the files:
-   roles/elasticsearch/defaults/main.yml
-   roles/kibana/defaults/main.yml
-   roles/fluentd/defaults/main.yml

To start the infrastracture 
*ansible-playbook -i inventory/hosts.ini playbooks/yourplaybook.yml*

To test if the stack is working you can use Vagrant.

To check if the cluster is working correctly you can perform the command curl -u elastic:yourpassword -k https://YourElasticHost:9200/_cluster/health or access from the Kibana Dashboard
