# Ansible Role: MSC

Installs and/or uninstalls software using the Managed Software Center (munki).

## Requirements
The machine upon which this role is running must have `managedsoftwareupdate` installed and in the path.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    msc_installs:   []
    msc_uninstalls: []

These contain the IDs of the apps to be (un)installed.

## Dependencies

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      vars:
        msc_installs:
          - anApp
          - another
        msc_uninstalls:
          - aThird 
      roles:
         - { role: deversmann.msc }

License
-------

MIT

Author Information
------------------

This role was created in 2021 by [Damien Eversmann](https://damien.live).
