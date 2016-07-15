setup-webserver-user-group
==========================

Add the "webserver_user" & configure owner permissions.

Requirements
------------

None.

Role Variables
--------------

- `APP_BASE_DIR` - the base, or root, of the application (where _owner_ is set)
- `WEBSERVER_USER` - name of the user associated with web server
- `VAGRANT` - indicate when operating within Vagrant; defaults to `False`

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - { role: setup-webserver-user-group,
            APP_BASE_DIR: "{{ TROPOSPHERE_LOCATION }}",
            tags: ['troposphere'] }

