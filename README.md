cdriehuys.virtualenv
=========

Create a python virtualenv.

Requirements
------------

None.

Role Variables
--------------

The following are the variables used by the role and their defaults.

```YAML
# How long the apt cache is valid after an update
apt_cache_time: 3600

venv: /opt/virtualenvs/venv     # Path to virtualenv
venv_packages: [python3]        # List of packages required to create the virtualenv
venv_python: python3            # Version of python to create the virtualenv with
venv_requirements: (undefined)  # If given, the virtualenv will have these packages installed

# Ownership settings
venv_owner: (undefined)
venv_group: (undefined)
```

Dependencies
------------

None.

Example Playbook
----------------

To run the role, include it as follows.

    - hosts: all
      roles:
         - cdriehuys.virtualenv

License
-------

MIT

Author Information
------------------

Chathan Driehuys (cdriehuys@gmail.com)
