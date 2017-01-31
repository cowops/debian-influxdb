Debian-Influxdb
===============

An open-source, distributed, time series database with no external dependencies.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

influxdb:
  version: 1.2.0
  port:
    admin: 8083
    api: 8086
    raft: 8090
    protobuf: 8099

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: loranger.debian-influxdb, influxdb.version: 1.2.0, influxdb.port.admin: 8083, influxdb.port.api: 8086, influxdb.port.raft: 8090, influxdb.port.protobuf: 8099 }

Tasks
-----

  - Install [InfluxDB](https://www.influxdata.com/time-series-platform/influxdb/)

License
-------

BSD
