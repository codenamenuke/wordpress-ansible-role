WordPress Role
=========
Ansible role for installing & configuring WordPress with Apache2 server on Ubuntu Systems.

Role Variables
--------------
This role only fetches MySQL user, password and DB name as variables from `defaults/main.yml`. You can create a separate vars.yml or a vars folder or directly mention your specific vars inside the main playbook and pass encrypted variables using Ansible Vault.

```yaml
my_sql_db: wordpress
my_sql_user: wordpress
my_sql_password: randompassword
```

Dependencies
------------
This role does not have any dependencies. All of the required dependencies are installed within the role.

Example Playbook
----------------
Here is an example Playbook.

```yaml
- hosts: wordpress
  gather_facts: False

  roles:
    - wordpress
```

Contributing
------------
Please feel free to open issues if you find any bugs, problems or if you see room for improvement. Also feel free to contact me anytime if you want to ask or discuss something.

Disclaimer
----------
This role is provided AS IS and I can and will not guarantee that the role works as intended, nor can I be accountable for any damage or misconfiguration done by this role. Study the role thoroughly before using it.

License
-------
MIT

Author Information
------------------
© 2023. Nyukeit. [nyukeit.dev](https://nyukeit.dev)
