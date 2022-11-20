# ansible

### e.g.


```/etc/zabbix/hosts
all:
  vars:
    ansible_python_interpreter: /usr/bin/python3
#    ansible_python_interpreter: /usr/bin/python

docker:
  hosts:
    xxx.xxx.xxx.xxx:
    yyy.yyy.yyy.yyy:

openresty:
  hosts:
    xxx.xxx.xxx.xxx:
    yyy.yyy.yyy.yyy:
```
