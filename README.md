nodejs
======

This role installs Node.js using [NodeSource](https://github.com/nodesource/distributions) repositories.

Role Variables
--------------

- `nodejs_major_version`: Major version to install (default: '5')
- `nodejs_minor_version`: Minor version and revision (e.g. '9.0') to install. If not set, latest package is installed (default: '')

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
          role: nodejs,
          nodejs_minor_version: '9.0'
        }

License
-------

MIT

[![Build Status](https://travis-ci.org/dpujadas/ansible-role-nodejs.svg?branch=master)](https://travis-ci.org/dpujadas/ansible-role-nodejs)
