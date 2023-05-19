ansible-scylla-monitoring
=========

Deploy Scylla Monitoring configured for a cluster, with or without Docker

Requirements
------------

- Ansible 2.8 or higher
- Python 3.x

Role Variables
--------------

Please check under `defaults/main.yml`, the variables are heavily commented


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: scylla-monitoring
      roles:
        - ansible-scylla-monitoring


# [TODO] Deprecated variables and how to migrate data
* scylla_monitoring_deploy_path: /opt/scylla-monitoring
* scylla_monitoring_data_path: "{{ scylla_monitoring_deploy_path }}/data"
* scylla_monitoring_config_path:  "{{ scylla_monitoring_deploy_path }}/config"
* scylla_monitoring_prom_rules_path:  "{{ scylla_monitoring_config_path }}/prom_rules"
* scylla_monitoring_alertdata_path: "{{ scylla_monitoring_deploy_path }}/alertdata"

License
-------

Apache

Author Information
------------------

Dan Yasny: https://github.com/dyasny
