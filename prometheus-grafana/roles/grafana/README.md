Role Name
=========

Role to install Grafana


Role Variables
--------------

    grafana_url: https://grafana-tart.gz-url
    grafana_checksum: grafana tar file checksum
    tmp: Directory to store downloaded files temporally


Example Playbook
----------------

    - hosts: servers
      roles:
         - role: grafana
           vars:
            grafana_url: https://dl.grafana.com/oss/release/grafana-10.3.1.linux-amd64.tar.gz
            grafana_checksum: sha256:f464241330b1d70546e992b89cfdaf8880c8898ac688d96257a74ffccccacbde
            tmp: /home/user/

License
-------

BSD

Author Information
------------------

Jesus Salas
