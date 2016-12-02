salandur.postfix
==============

[![Build Status](https://travis-ci.org/salandur/salandur.postfix.svg?branch=master)](https://travis-ci.org/salandur/salandur.postfix)

Ansible role which manage postfix

### Usage

Add `salandur.postfix` to your roles and set vars in your playbook file.

Example:

```yaml
- hosts: all

  roles:
    - salandur.postfix

  vars:
    postfix_relayhost: "[your-mail-provider]:25"
```

### Variables

```yaml
postfix_hosttype: "localhost"
postfix_relayhost: smtp.example.com
postfix_test_email_address: test@example.com
```

#### Setting `postfix_hosttype`
If the host type is set to localhost, postfix will only listen to local connections. This is the default.
Any other value will turn this into an internet host. 

### License

Licensed under the MIT License. See the LICENSE file for details.

### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/salandur/salandur.postfix/issues)!
