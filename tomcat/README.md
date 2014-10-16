# tomcat 

- Does a basic install of tomcat, configures log rotation, installs java, creates a tomcat user and sets appropriate permissions 

## supported platforms

- CentOS

## Role Variables

- user_shell: defaults to "/bin/bash", modify this if shell is in a non default location
- tomcat_version: defaults to "7.0.56", can be changed to any version stored as a tar.gz in /opt/ansible_store/tomcat
- java_opts: defaults to null
- catilina: defaults to null
- catilina_pid: defaults to "/opt/tomcat/catalina.pid", location of the tomcat pid file
- mat_threads: defaults to 10, determines the maximum number of threads to serve your tomcat app
- management_address: defaults to "127.0.0.1", this address SHOULD NOT BE PUBLIC
- app_address: defaults to "127.0.0.1", what ip your app should listen, 127.0.0.1 assumes you're putting this behind a webserver (ex. apache,nginx)
- jvmroute: defaults to "default", for configuring mod_jk
- server_info: defaults to null
- server_number: defaults to null
- server_built: defaults to null

## Manages

- /opt/tomcat/bin/catalina.sh
- /opt/tomcat/conf/server.xml
- /etc/init.d/tomcat
- /etc/logrotate.d/tomcat
- /etc/tomcat/lib/org/apache/catalina/util/ServerInfo.properties
- tomcat user
- tomcat log rotation
- tomcat permissions
- tomcat service

## Role Dependencies

- custom
- logrotate
- java

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: tomcat 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
