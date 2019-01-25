[![Build Status](https://travis-ci.com/calvinbui/ansible-mongodb.svg?branch=master)](https://travis-ci.com/calvinbui/ansible-mongodb)

# Ansible MongoDB

MongoDB for Ubuntu. Made to follow the [official guide](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/).

Not every version of MongoDB is available for every version of Ubuntu. Therefore the variable `mongodb_ubuntu_version` can be used to install older MongoDB versions on newer Ubuntu hosts.

##  Requirements

N/A

## Role Variables

`mongodb_version`: Version of mongodb to install. Must be exact.

`mongodb_ubuntu_version`: Mirror to use. Not every mirror is available for every version.

## Dependencies

N/A

## Example Playbook

```yaml
- hosts: servers
  become: true
  roles:
    - role: calvinbui.ansible_mongodb
```

## License

GPLv3

## Author Information

http://calvin.me
