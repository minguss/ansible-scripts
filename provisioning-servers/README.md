# How to use?

Step 1. Clone git repo
---
``` bash
git clone https://github.com/minguss/ansible-scripts.git && cd ansible-scripts/provisioning-servers
```

Step 2. Fill out inventory file parameter
---
``` bash
[servers]
ansible2 # you can replace ip-addr
ansible3


[all:vars]
ansible_connection=ssh
ansible_ssh_user=[ssh-name]
ansible_ssh_pass=[password]
ansible_sudo_pass=[password]
```

Step3. Execute ansible-playbook
---
``` bash
ansible-playbook -i hosts ping.yml
```
![222](https://user-images.githubusercontent.com/22410442/66102004-c9f71800-e5eb-11e9-95e2-6736f8835aaa.png)
