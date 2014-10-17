# logrotate 

- Sets basic log rotation in place. 

## supported platforms

- CentOS

## Role Variables

- none 

## Manages

- logrotate
- cleaning up after CentOS 

## Role Dependencies

- custom

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: logrotate 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
