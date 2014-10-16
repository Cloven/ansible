# loader 

- Checks to see if the box is virtual or pysical and then loads the required modules. 

## supported platforms

- FreeBSD

## Role Variables

- none 

## Manages

- /boot/loader.conf 

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: loader 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
