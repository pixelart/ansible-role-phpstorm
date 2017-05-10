# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) 
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]
### Added
- Create PhpStorm command line launcher `pstorm`

### Changed
- Finally deactivate the automated update checks

## [1.0.2] - 2017-05-09
### Changed
- Update default PhpStorm version to 2017.1.3

## [1.0.1] - 2017-02-07
### Fixed
- Set inotify limit to 512K which is needed by PhpStorm

## [1.0.0] - 2017-02-01
### Added
- Created the role to provision the Jetbrains PhpStorm IDE
- Add variables to define the installed PhpStorm version and install path
- Test the role on CentOS 7, Fedora 2.4, Ubuntu 16.04 and Debian 8

[Unreleased]: https://github.com/pixelart/ansible-role-phpstorm/compare/1.0.2...HEAD
[1.0.2]: https://github.com/pixelart/ansible-role-phpstorm/compare/1.0.1...1.0.2
[1.0.1]: https://github.com/pixelart/ansible-role-phpstorm/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/pixelart/ansible-role-phpstorm/compare/d4b3ad1...1.0.0
