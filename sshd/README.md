# sshd 

- A simple role to ensure that pf(FreeBSD firewall) is managed 

## supported platforms

- FreeBSD
- CentOS

## Role Variables

- none 

## Manages

- sshd_config: base sshd configuration file 

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: sshd 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
