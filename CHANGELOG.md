# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0] - 2020-07-20

[Full Changelog](https://github.com/jpylypiw/easywall/compare/v0.1.0...v0.2.0)

### Added

- GitHub sponsorship was activated for the project
- A large number of configuration entries have been added
- Blocked connections can be logged by iptables
- Connections from blacklisted senders can be logged
- Broadcast, multicast and anycast packets can be blocked
- SSH brute force prevention was added. Attention! The feature is in alpha state and untested
- ICMP flood prevention has been implemented. The feature is also in alpha state
- Drop Invalid Packages was implemented. This is also an Alpa version
- Port Scan Prevention has been implemented. The feature is currently unstable in my tests
- IPv6 Router Advertisement connections can be allowed or prohibited
- IPv6 Neighbor Advertisement packets can also be allowed or prohibited
- Installation and update documentation has been improved
- easywall is now programmed completely typed thanks to mypy
- Ports can now be forwarded from the local system. Note that both the source and destination ports must be opened. This is because this is only a nat forwarding and not a FORWARDING forwarding
- The translations have been significantly improved thanks to deepl.com
- Username and password for the web interface can be changed directly in the web interface
- It is recognized if configuration entries are missing. This is especially important in this version, because we have added some variables. You will be notified about the differences in the web interface
- The start page of the web interface has been completely reworked. In the future I imagine a tag cloud from the open ports
- The options page in the web interface now contains almost all settings from the files

### Changed

- Python 3.5 is no longer supported, because no typing of variables is possible
- The detection from the first start has now been changed to a detection at every start. This has proven to be useful, as more rule types may be added in the future.
- The configuration files are reloaded each time a variable is called. This is needed to activate changes from the web interface immediately.
- An additional Python package "natsort" is required. The package offers the possibility to sort the ports naturally.
- The allowed ICMPv4/v6 types are now strongly restricted.

Allowed ICMPv4 types:

- 0 echo-reply
- 3 destination-unreachable
- 11 time-exceeded
- 12 parameter problem

Allowed ICMPv6 types:

- 1 destination-unreachable
- 2 packet-too-big
- 3 time-exceeded
- 4 parameter problem
- 128 echo request
- 129 echo-reply

After explicit configuration the following ICMPv6 types are allowed additionally:

- 133 router solicitation
- 134 router advertisement
- 135 neighbor solicitation
- 136 neighbor advertisement

## [0.1.0] - 2020-06-21

[Full Changelog](https://github.com/jpylypiw/easywall/compare/v0.0.4...v0.1.0)

### Added

- This version is almost completely tested by unit tests.
- The documentation was completely revised and can now be found in the `docs` folder.
- The configuration has been shortened and simplified.
- The installation, uninstallation and an update can now be carried out via scripts.
- The web interface installation now creates self-signed SSL certificates and can only be used over HTTPS.

### Changed

- create a setup.py and setup.cfg file for publishing
- create a requirements.txt file with all the requirements
- create github actions testing and linting
- implement custom rules feature
- create unit tests for all classes in easywall folder
- create unit tests for all classes in web folder
- rework all classes in easywall folder
- rework all classes in web folder
- set up a demo server
- write documentation for development setup
- SSL Implementation for web application
- write documentation for installing and uninstalling

## [0.0.4] - 2019-10-04

[Full Changelog](https://github.com/jpylypiw/easywall/compare/v0.0.3...v0.0.4)

### Added

- added possibility to apply custom IPTables rules
- full implemented webinterface - old PHP sources are history
- rule changes made in the webinterface are only written temporary into web directory
- rules can be applied in the webinterface
- a lot of code improvements
- this is kind the first "stable" version ready for testing
- I will test this on my webserver a lot, so the next versions will be more stable

### Changed

- too many, I can't count them
- there was a long time since the last version

## [0.0.3] - 2019-06-30

[Full Changelog](https://github.com/jpylypiw/easywall/compare/v0.0.2...v0.0.3)

### Added

- added easywall-Web using flask
- added old php templates to web
- improved install script a lot and added so many features to it
- simplified code using codacy and code climate
- ICMP Support added after testing on a server of mine
- added a daemon script for running easywall-Web
- 404 error page added to web
- for a production use of easywall-Web I added uwsgi instead of the small development server of flask
- logout button added to web
- added a password generator script and added it to install script

### Changed

- improved exception handling in several files
- the `.running` file was not deleted properly
- moved the system `os.system` to a single function where security checks can be implemented in the future

## [0.0.2] - 2019-06-08

[Full Changelog](https://github.com/jpylypiw/easywall/compare/v0.0.1...v0.0.2)

### Added

- Changed branch master to old python branch
- Renamed old master branch to php-old
- Bumped version
- Changed documentation

### Changed

- Information of the user in install.sh if not running as root or using sudo
- Removed quiet option in install.sh for apt-get and pip3 for better user experience

## [0.0.1] - 2019-04-24

### Added

- Incomplete Rework of Branch php-old
- easywall is split in two parts in the new concept
- easywall Firewall Core Part running as root user finished
- The New easywall will be one part running as root and one part running as easywall user which has access to config files.

[unreleased]: https://github.com/jpylypiw/easywall/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/jpylypiw/easywall/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/jpylypiw/easywall/compare/v0.0.4...v0.1.0
[0.0.4]: https://github.com/jpylypiw/easywall/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/jpylypiw/easywall/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/jpylypiw/easywall/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/jpylypiw/easywall/releases/tag/v0.0.1
