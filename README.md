ansible-hel-nginx
=================

ansible-hel-nginx is a role for setting up nginx as front for different
types of web applications. Specifically it supports:

* uwsgi sockets, for applications running inside UWSGI
* reverse proxying to HTTP
* static file bundles, with try_files returning the index
* static file aliases for supporting files

Role Variables
--------------

There are a whole set lot settings for this role. The most interesting are:

* nginx_uwsgis: uwsgi services
* nginx_proxies: HTTP services
* nginx_tryfiles: static files bundles with specified default response
* nginx_aliases: plain nginx aliases

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

ville.koivunen@hel.fi
