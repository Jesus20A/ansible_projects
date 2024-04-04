Role Name
=========

Role to install node exporter for Prometheus


Role Variables
--------------

    node_exporter_url: https://node-exporter-tart.gz-url
    node_exporter_checksum: node exporter tar file checksum
    tmp: Directory to store downloaded files temporally


Example Playbook
----------------

    - hosts: servers
      roles:
         - roles: node-exporter
           vars:
            node_exporter_url: https://github.com/prometheus/node_exporter/releases/download/v1.7.0/node_exporter-1.7.0.linux-amd64.tar.gz
            node_exporter_checksum: sha256:a550cd5c05f760b7934a2d0afad66d2e92e681482f5f57a917465b1fba3b02a6
            tmp: /home/user/

License
-------

BSD

Author Information
------------------

Jesus Salas
