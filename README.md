Rabbitmq-grafana playbook
=========

This playbook installs and configure RabbitMQ, Prometheus and Grafana.

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
