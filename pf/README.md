# pf 

- A simple role to ensure that pf(FreeBSD firewall) is managed 

## supported platforms

- FreeBSD

## Role Variables

- pf_enabled: defaults to "no", set to yes if you want the pf firewall to be enabled

## Manages

- /etc/pf.conf 

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: pf 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
