salandur.postfix
==============

Ansible role which manage postfix

#### Usage

Add `salandur.postfix` to your roles and set vars in your playbook file.

Example:

```yaml
- hosts: all

  roles:
    - salandur.postfix

  vars:
    postfix_relayhost: "[your-mail-provider]:25"
```

#### License

Licensed under the MIT License. See the LICENSE file for details.

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/salandur/salandur.postfix/issues)!
