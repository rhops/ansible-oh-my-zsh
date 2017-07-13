An Ansible role to install [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) for *ANY* user.

### Dependencies
None

### Tested Environment
* Ansible 2.1
* CentOS 6/7

### Installation
```
ansible-galaxy install rhops.oh-my-zsh
```

### Role Variables
All the available options are not mandatory at the moment. Default values could be  referenced from the [role's defaults directory](defaults/main.yml).


* Use customized repo other than the official one.

```
oh_my_zsh_repo: https://github.com/robbyrussell/oh-my-zsh
```

* Specify list of users whom the Oh My Zsh is intended for.

```
oh_my_zsh_users:
  - "{{ ansible_ssh_user }}"
  - root
```

* Whether to backup existing `.zshrc` or not

```
oh_my_zsh_backup_zshrc: yes
```
### License
Apache 2.0

### Author Information

This role was created in 2017 by [Jeff Li](http://blog.jeffli.me)

