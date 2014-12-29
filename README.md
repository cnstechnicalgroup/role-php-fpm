Role: cns.php-fpm
========

This role installs and configures php-fpm (debian).

Requirements
------------

Nothing, it runs out of the box.

Role Variables
--------------

In the current version, you can specify the following variables:

| Name                  | Default |                                                              |
|-----------------------|---------|--------------------------------------------------------------|
| web_root              |   ---   | Main root for prestashop install.  (full system path)        |
| web_folder            |   ---   | Site folder name. (not full path)                            |
| site_public_url       |   ---   | Site URL. The primary site URL.                              |
| phpfpm_process_user   |   ---   | php-fpm process owner.                                       |
| phpfpm_process_group  |   ---   | php-fpm process group.                                       |

Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by Sam Morrison
https://www.twitter.com/samcns

Examples
--------

```yaml
---
- name: common role test
  hosts: all
  roles:
    - cns.php-fpm
```
