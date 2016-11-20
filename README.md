squads.postfix
==============

Ansible role which manage postfix

#### Usage

Add `squads-postfix` to your roles and set vars in your playbook file.

Example:

```yaml

- hosts: all

  roles:
    - squads-postfix

  vars:
    # Example configuration for gmail
    postfix_relayhost: "[smtp.gmail.com]:587"

```

#### License

Licensed under the MIT License. See the LICENSE file for details.

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/salandur/squads-postfix/issues)!
