# limits.d 

- basically makes everything unlimited because thats the standard configuration around these parts -_-

## supported platforms

- CentOS

## Role Variables

- none 

## Manages

- Role only works on RedHat based systems
- Places custom.conf in /etc/secuirty/limits.d
- Ensure the privileges are correct on /etc/security/limits.d and intermedix.conf

## Role Dependencies

- custom

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: limits.d 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
