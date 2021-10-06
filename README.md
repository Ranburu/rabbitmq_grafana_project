Rabbitmq-grafana playbook
=========

This playbook installs and configure RabbitMQ, Prometheus and Grafana.

Role Variables
--------------



Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - hosts: rabbitmq
      remote_user: root

      roles:
      - rabbitmq_install
      - rabbitmq_setup

    - hosts: monitoring
      remote_user: root
      
      roles:
      - prometheus
      - grafana

License
-------

BSD

Author Information
------------------

Dmitry Shorokhov