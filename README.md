 The following is handled out of the box:

* User setup
* SSH hardening
* Firewall setup

It will also install the following software:

* Nginx with HTTP/2
* PHP 8.1
* MySQL
* Redis
* WP-CLI
* Fail2Ban

## Usage

Configure your [hosts file](https://github.com/deliciousbrains/wordpress-ansible/blob/master/hosts).

```
[production]
10.99.99.28  
```

Edit [provision.yml](https://github.com/deliciousbrains/wordpress-ansible/blob/master/provision.yml) to configure your default user, [hashed](https://docs.ansible.com/ansible/latest/reference_appendices/faq.html#how-do-i-generate-encrypted-passwords-for-the-user-module) sudo password and local public key path. This will create a new user on the provisioned servers that you can use to gain SSH access.

Run:

`test.yml`
