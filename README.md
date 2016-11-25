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

#### Variables

```yaml
postfix_mailer_type: "Satellite system"
postfix_myhostname: "{{ansible_hostname}}"
postfix_relayhost: smtp.example.com
postfix_test_email_address: test@example.com
```

#### Setting `postfix_mailer_type`

* **Internet Site**: Mail is sent and received directly using SMTP.
* **Internet with smarthost**: Mail is received directly using SMTP or by running a utility such as fetchmail. Outgoing mail is sent using a smarthost.
* **Satellite system**: All mail is sent to another machine, called a 'smarthost', for delivery.  
* **Local only**: The only delivered mail is the mail for local users. There is no network.
 

#### License

Licensed under the MIT License. See the LICENSE file for details.

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/salandur/salandur.postfix/issues)!
