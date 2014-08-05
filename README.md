ansible-role-build-essential
========

Ansible role which installs packages required for compiling C software from source.

This is a fork of [Ansibles/build-essential](https://github.com/Ansibles/build-essential). The upstream seems not updated very often, so I forked.

## Usage

Install from ansible-galaxy

```shell
$ ansible-galaxy install -p . kun432.build-essential
```
or from github.

```shell
$ git clone https://github.com/kun432/ansible-role-build-essential.git kun432.build-essential
```

Create a playbook(ex.`localhost.yml`) and a inventory(ex.`hosts`) in same directory you install role.

###### hosts
```
localhost
```
 
###### localhost.yml
```yml
- hosts: localhost
  connection: local
  sudo: yes
  roles:
    - kun432.build-essential
```
Run.
```shell
$ ansible-playbook -i hosts localhost.yml
```

## Requirements & Dependencies

- Tested on Ansible 1.6.6.
- Tested for the following OS:
 - Debian 7.0 (wheezy)
 - Ubuntu 10.04
 - Ubuntu 12.04.4
 - Ubuntu 14.04
 - CentOS 5.8
 - CentOS 6.5
 - CentOS 7.0
 - Fedora 19
 - Fedora 20
 - OpenSUSE 13.1
 - FreeBSD 10

## Variables

None,

## License

Licensed under the MIT License.

## Contribute

Feedback, Tests, bug-reports and requests are always [welcome](https://github.com/kun432/ansible-role-build-essential/issues)!

