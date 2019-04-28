# ansible-role-influxdb

[![Build Status](https://travis-ci.org/BadFever/ansible-role-influxdb.svg?branch=master)](https://travis-ci.org/BadFever/ansible-role-influxdb)

Install and configure influxdb.

## Requirements

None.

## Role Variables

A lot.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: influxdb-servers
  remote_user: root
  roles:
    - ansible-role-influxdb
```

## License

MIT

## Firewall

```bash
# client-server communication using the InfluxDB HTTP API.
firewall-cmd --add-port=8086/tcp --permanent
# RPC service to perform back up and restore operations.
firewall-cmd --add-port=8088/tcp --permanent
firewall-cmd --reload
```
