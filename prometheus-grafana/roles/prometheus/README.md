Role Name
=========

Role to install Prometheus


Role Variables
--------------

    prometheus_url: https://prometheus-tart.gz-url
    prometheus_checksum: prometheus tar file checksum
    tmp: Directory to store downloaded files temporally


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: prometheus
           vars:
            prometheus_url: https://github.com/prometheus/prometheus/releases/download/v2.49.1/prometheus-2.49.1.linux-amd64.tar.gz
            prometheus_checksum: sha256:93460f66d17ee70df899e91db350d9705c20b1576800f96acbd78fa004e7dc07
            tmp: /home/user/
            
License
-------

BSD

Author Information
------------------

Jesus Salas
