# motd 

- A simple role to push out the standard message of the day 
- YOU WILL NEED TO MODIFY THE MOTD TEMPLATE

## supported platforms

- FreeBSD
- CentOS

## Role Variables

- none 

## Manages

- /etc/motd 

## Role Dependencies

- custom

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: motd 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
