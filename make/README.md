# make 

- A simple role to push make.conf out to FreeBSD systems. 

## supported platforms

- FreeBSD

## Role Variables

- none 

## Manages

- /etc/make.conf 

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: make 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
