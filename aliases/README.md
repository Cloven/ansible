# aliases 

- Unifies aliases file so both FreeBSD and CentOS work with the same file. rebuilds aliases if changed. 

## supported platforms

- CentOS
- FreeBSD

## Role Variables

- admin_emails: This should be modified in your base vars file included in your base playbook 

## Manages

- unified Linux and FreeBSD aliases file 

## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: aliases 
```
## License

MIT

## Author Information

Tony Welder
