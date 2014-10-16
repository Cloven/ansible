# java 

- a role of capable of installing multiple Java installations at the same time.  Configuration symbolic links for default and latest in /usr/java.  sets JAVA_HOME and JRE_HOME via java.sh in /etc/profile.d.  Also adds java to the paths when a profile is loaded 

## supported platforms

- CentOS

## Role Variables

- default: default is "latest", where the symbolic link for /usr/java/default should point
- latest: default is "jre1.7.0_67", where the symbolic link for /usr/java/latest should point
- java_versions: default is "jre1.7.0_67",a list of java versions to be installed, (COMPLETLY dependent on having a /opt/ansible_store/java/ dir with compressed JREs store in it)
  - "jre1.7.0_67"

- java_home: default is "/usr/java/default", variable is used in /etc/profile.d/java.sh to set the JAVA_HOME environmental variable
- jre_home: default is "/usr/java/default/jre", variable is used in /etc/profile.d/java.sh to set the JRE_HOME environmental variable


## Manages

- /etc/profile.d/java.sh 
- /usr/java
- java verisons
- java search pathes


## Role Dependencies

- custom 

## Example Playbook

```yaml
- hosts: all
  sudo: yes
  roles:
    - role: java 
```
## License

- MIT

## Author Information

- Tony Welder
- tony.wvoip@gmail.com
