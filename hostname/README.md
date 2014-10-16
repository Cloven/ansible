# hostname 

- Sets hostname on FreeBSD/CentOS 

## supported platforms

- CentOS
- FreeBSD

## Role Variables

- none: it sets the inventory_hostname as your hostname (don't use FQDN... seriously guys, use facility qualified)

## Manages

- hostname 

## Role Dependencies

- none

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: hostname 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
