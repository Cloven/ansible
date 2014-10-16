# iptables 

- A simple role to disable/enable iptables. 

## supported platforms

- CentOS

## Role Variables

iptables_enabled: defaults to "no", can also be set to yes

## Manages

- iptables service 
- /etc/sysconfig/iptables

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: iptables 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
