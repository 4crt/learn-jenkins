# Prerequisites
You are able to connect to target nodes via SSH (with privileged user) and create ansible user with below command:
```
ansible all -u <default_privileged_user> -m user -a "name=ansible"
```
Target nodes are reachable with 'ansible' user via SSH

# Tips
Make sure permissions for SSH folder and it's contents are set correspondingly

Make sure privileges of 'ansible' may be escalated
```
ansible all -u <default_privileged_user> -m copy -a "src=./tmp/sudoers dest=/etc/sudoers.d/ansible"
```

To list available modules (for newer versions)
```
ansible-doc -t module -l
```

To read docs about module
```
ansible-doc <module>
```
