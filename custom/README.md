# custom 

- creates /usr/local/ansible for custom files, scripts and configuration 

## supported platforms

- CentOS
- FreeBSD

## Role Variables

- none 

## Manages

- /usr/local/ansible/ansible_backup_cleanup.sh : ansible backup clean up script 
- /usr/local/ansible

## Role Dependencies

- none 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: custom 
```
## License

MIT

## Author Information

Tony Welder
