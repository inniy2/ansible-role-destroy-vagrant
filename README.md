## Destroy vagrant  

- - - -  
#### Version dependency  
1. Ansible: `2.5.1`
2. Python:  `3.6.5`


- - - -  
#### Role dependency  
`ansible-role-deploy-vagrant`


- - - -  
#### VARS
```
None
```

- - - -  
#### Playbook example  


```yml
---
- hosts: workstation
  become: no

  environment:
    PATH: "/usr/local/bin:{{ ansible_env.PATH }}:$PATH"

  roles:
    - ansible-role-destroy-vagrant
```



