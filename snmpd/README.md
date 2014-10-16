# snmpd 

- A role to manage the snmpd service and configuration 

## supported platforms

- CentOS
- FreeBSD

## Role Variables

- auth_community: defaults to "default", should change this if you have authorized community configured on your snmp trap 

## Manages

- snmpd.conf: base configuration file for snmpd 

## Role Dependencies

- custom 
- hostname

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: snmpd 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
