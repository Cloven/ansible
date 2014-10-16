# sudoers 

- Manages the sudoer's file, gives wheel group root access and enables sudoers.d 

## supported platforms

- CentOS
- FreeBSD

## Role Variables

- none

## Manages

- /etc/sudoers or /usr/local/etc/sudoers 

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: sudoers 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
