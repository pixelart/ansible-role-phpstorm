# Ansible Role: PhpStorm

[![Build Status](https://travis-ci.org/pixelart/ansible-role-phpstorm.svg?branch=master)](https://travis-ci.org/pixelart/ansible-role-phpstorm)

Installs the [Jetbrains PhpStorm IDE](https://www.jetbrains.com/phpstorm/), on any Linux or UNIX system.

## Requirements

  - `java` should be installed and working.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    phpstorm_version: '2017.1.3'

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

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## License

MIT, see the [LICENSE](LICENSE) file.

## Author Information

This role was created in 2017 by [pixelart GmbH](https://www.pixelart.at/).
