# Ansible Role: PhpStorm

[![Build Status](https://travis-ci.org/pixelart/ansible-role-phpstorm.svg?branch=master)](https://travis-ci.org/pixelart/ansible-role-phpstorm)

Installs the [Jetbrains PhpStorm IDE](https://www.jetbrains.com/phpstorm/), on any Linux or UNIX system.

## Requirements

  - `java` should be installed and working.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    phpstorm_version: '2017.1.3'

The version of PhpStorm which should be installed.

    phpstorm_install_basepath: '/opt/jetbrains'

The base path where PhpStorm will be installed.

    phpstorm_install_prefix: 'phpstorm'
    
The prefix of the installation folder within the installation path. Together with `phpstorm_version` and `phpstorm_install_basepath` this will result in the following default install path: `/opt/jetbrains/phpstorm-2017.1.3`.

    phpstorm_commandline_launcher: 'pstorm'
    
The executable name of the command-line launcher. Set to `False` if you don't want to install one.

    phpstorm_cleanup_releases: []
    
Version number of old PhpStorm releases you want to delete. It is important to not change `phpstorm_install_basepath` and `phpstorm_install_prefix` between installation if want to cleanup. Otherwise old versions won't be found.

Side note: Never delete the version from whom you are upgrading. It may be opened by a developer and this will lead to crashes.

## Dependencies

None.

## Example Playbook

    - hosts: phpdevs
      roles:
        - pixelart.phpstorm

After the playbook runs, PhpStorm will be installed, and an application and a command-line launcher will be accessible via normal user accounts.

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## License

MIT, see the [LICENSE](LICENSE) file.

## Author Information

This role was created in 2017 by [pixelart GmbH](https://www.pixelart.at/).
