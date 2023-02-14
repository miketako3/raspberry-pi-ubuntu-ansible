# Ansible For Raspberry Pi and Ubuntu Server
- apt update
- send ssh public key
- change ssh port from 22 to 2222
- configure ufw
- configure wifi and static ip

# Usage

## Turn on Raspberry Pi

- connect lan cable
- connect power cable
- `ssh ubuntu@${IP_ADDRESS}`
- change password from default to any string

## Prepare files

- hosts
  - copy sample file
- private.yml
  - ${PROPERTY}: ${EXAMPLE}
  - SSH_PORT: 2222
  - SERVER_IP_ADDRESS: 192.168.0.10/24 
  - ROUTER_IP_ADDRESS: 192.168.0.1 
  - NAME_SERVER_IP_ADDRESS: 192.168.0.1 
  - ACCESS_POINT_SSID: foobar
  - ACCESS_POINT_PASSWORD: wifipassword

## Start Ansible Script

```shell
$ docker-compose up
```