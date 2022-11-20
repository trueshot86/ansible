# ansible

### e.g.

/etc/ansible/hosts

```
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

実行
```
$ ansible-playbook hoge.yml --ask-pass -e "domain=fuga.com"
```


警告メッセージ回避

/etc/ansible/ansible.cfg
```
[ssh_connection]
ssh_args = -o ControlMaster=auto -o ControlPersist=60s -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null
```


