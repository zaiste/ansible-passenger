ansible-passenger
=========

Ansible role that installs Phusion Passenger for Ubuntu from the official APT.

Requirements
------------

None.

Role Variables
--------------

- `dist` defaults to `artful`

- `nginx_worker_connections` defaults to `768`;
- `nginx_keepalive_timeout` defaults to `65`;
- `nginx_server_names_hash_bucket_size` defaults to `64`;
- `nginx_server_name` defaults to `app.example.com`

- `passenger_app_env` defaults to `production`
- `passenger_app_root` defaults to `/srv/app/public`
- `passenger_app_vars` is a list of `name` and `value` pairs

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: servers
  roles:
  - role: zaiste.passenger
    passenger_app_vars:
    - name: RAILS_ENV
      value: production
```

License
-------

MIT / BSD

Author Information
------------------

[Zaiste](http://zaiste.net) 2017 
