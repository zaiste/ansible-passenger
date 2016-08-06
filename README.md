ansible-passenger
=========

Ansible role that installs Phusion Passenger for Ubuntu Xenial from the official APT.

Requirements
------------

None.

Role Variables
--------------

- `nginx_worker_connections` defaults to `768`;
- `nginx_keepalive_timeout` defaults to `65`;
- `nginx_server_names_hash_bucket_size` defaults to `64`;
- `nginx_server_name` defaults to `app.example.com`

- `passenger_app_env` defaults to `production`
- `passenger_app_root` defaults to `/srv/app/public`

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: zaiste.passenger }

License
-------

MIT / BSD

Author Information
------------------

[Zaiste](http://zaiste.net) 2014 - 2016
