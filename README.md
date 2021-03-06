# otto-install

Installs [Hashicorp's Packer](https://ottoproject.io)



## Role Variables
```yml

---
app:
  name: otto
  version: 0.1.2

install:
  dir : /usr/local/bin
  download_location: https://releases.hashicorp.com/otto
  file_list:
    - otto

```


Example Playbook
----------------
```yml

---
- hosts: local
  sudo: true
  gather_facts: true

  roles:
    - marcelocorreia.otto-install

  vars_files:
    - ../vars/tardis.yml

```

License
-------

MIT

Author Information
------------------
Some useful stuff at:
  - [https://github.com/marcelocorreia](https://github.com/marcelocorreia)
  - [https://galaxy.ansible.com/list#/users/15516](https://galaxy.ansible.com/list#/users/15516)
  - [https://hub.docker.com/u/marcelocorreia/](https://hub.docker.com/u/marcelocorreia/)
  - Any issues, pull-request are welcome
