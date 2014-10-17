# nagios 

- manages nrpe, the config files, and the sudoers file 

## supported platforms

- FreeBSD
- CentOS

## Role Variables

- pid_file:  defaults to "/var/run/nrpe.pid", determines the location of the nrpe pid file
- server_port: default is 5666, determins the port that nrpe listens on
- nrpe_user: defaults to "nagios", change this if you don't want the user to be nagios
- nrpe_user: defaults to "nagios", determins the group for nrpe daemon
- dont_blame_nrpe: defaults to 1, enables remote exectuion of scripts.... is considered insecure to have this enabled
- debug: defaults to 0, changes log level to debug
- command_timeout: defaults to 200, number of seconds to wait for a check to finish executing
- allowed_hosts: defaults to 127.0.0.1, should be a comma seperated list of nagios slaves 

## Manages

- nrpe.cfg: nagios client configuration file
- Nagios sudoers file
- NRPE service

## Role Dependencies

- custom
- sudoers 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: nagios 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
