Ulimit
=========

Allows controlling ulimit parameters.

Role Variables
--------------

```
ulimit_config: []
```

Example Variables
----------------

```
ulimit_config:
    - domain: '*'
      limit_type: 'soft'
      limit_item: 'nofile'
      value: 65536
    - domain: '*'
      limit_type: 'hard'
      limit_item: 'nofile'
      value: 65536
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: silverlogic.ulimit }

License
-------

Apache 2.0
