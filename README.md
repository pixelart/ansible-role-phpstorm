# Ansible Role: PhpStorm

[![Build Status](https://travis-ci.org/pixelart/ansible-role-phpstorm.svg?branch=master)](https://travis-ci.org/pixelart/ansible-role-phpstorm)

Installs the [Jetbrains PhpStorm IDE](https://www.jetbrains.com/phpstorm/), on any Linux or UNIX system.

## Requirements

  - `java` should be installed and working.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    phpstorm_version: '2016.3.2'

The version of PhpStorm which should be installed.

    phpstorm_install_path: '/opt/jetbrains/phpstorm-{{ phpstorm_version }}'

The path where PhpStorm will be installed and available to your system.

## Dependencies

None.

## Example Playbook

    - hosts: phpdevs
      roles:
        - pixelart.phpstorm

After the playbook runs, PhpStorm will be installed, and an application launcher will be accessible via normal user accounts.

## License

MIT, see the [LICENSE](LICENSE) file.

## Author Information

This role was created in 2017 by [pixelart GmbH](https://www.pixelart.at/).
