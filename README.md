# easywall

[![GitHub Actions Build](https://img.shields.io/github/workflow/status/jpylypiw/easywall/python-testing)](https://github.com/jpylypiw/easywall/actions)
[![Coveralls github](https://img.shields.io/coveralls/github/jpylypiw/easywall)](https://coveralls.io/github/jpylypiw/easywall)
[![GitHub license](https://img.shields.io/github/license/jpylypiw/easywall)](https://github.com/jpylypiw/easywall/blob/master/LICENSE)
[![GitHub repo size](https://img.shields.io/github/repo-size/jpylypiw/easywall.svg)](https://github.com/jpylypiw/easywall)
[![Project Version](https://img.shields.io/badge/release-development-red.svg)](https://github.com/jpylypiw/easywall)
[![Discord Support](https://img.shields.io/discord/333980251921186818)](https://discord.gg/CUj2sFb)
[![Beerpay](https://img.shields.io/beerpay/jpylypiw/easywall)](https://beerpay.io/jpylypiw/easywall)

Today **Firewalls** are more important than years before. Hackers and Bots are trying to invade your server. So what is the most effective way to prevent this?
Set up a firewall! But which one? **IPTables** is the strongest firewall in **Linux** environments. So we wanted to make IPTables usable by everyone. We created a simple **Web Interface** for IPTables so everyone can install and use it on his / her server.

## Features

- Configuration of Firewall Rules using a **simple Webinterface**
- **Blacklist** for blocking incoming triffic from a IPV4 / IPV6 Address
- **Whitelist** to allow all incoming network traffic from a specific IP Address
- Allow incoming traffic to a **single TCP or UDP Port**
- Allow incoming Traffic from a **TCP or UDP Port range**
- **Automatic Reset of Firewall Settings** on connection loss or bad firewall settings

## Demo

You can view an online version of the program as a demo under the following link:

<https://dev01vt.wdkro.de:12227/> (Certificate is provided by Let's Encrypt)

- **Username**: demo
- **Password**: demo

The online demo version is reset every 30 minutes and all data is deleted. The demo has only the frontend installed without the backend. Configuration changes are therefore not saved or applied.

## Roadmap for the next release

Most of you noticed that there are a lot of changes made at the moment, but the release status is still in "development" and there are no minor releases. This is because I currently enhance the project until the next release. The reason for this is because I learned a lot of Python 3 coding the last year in my main job. I want to use this knowledge and clean this project up so everyone can use it and there are less bugs than before (there were a lot of bugs). If you want to support me and improve the development speed you can send me a beer on beerpay :beers:

- :heavy_check_mark: create a setup.py and setup.cfg file for publishing
- :heavy_check_mark: create a requirements.txt file with all the requirements
- :heavy_check_mark: create github actions testing and linting
- :heavy_check_mark: implement custom rules feature
- :heavy_check_mark: create unit tests for all classes in easywall folder
- :heavy_check_mark: create unit tests for all classes in web folder
- :heavy_check_mark: rework all classes in easywall folder
- :heavy_check_mark: rework all classes in web folder
- :heavy_check_mark: set up a demo server
- :heavy_check_mark: write documentation for development setup
- :heavy_check_mark: SSL Implementation for web application
- :heavy_check_mark: write documentation for installing and uninstalling

## Roadmap for later version

These are long-term planned features. If you want to have more features listed here you just have to create a issue and we can discuss the feature.

- :x: create a `pydoc` documentation
- :x: finish all `TODO: Docs` documentations
- :x: create a ansible role for easy installing
- :x: fill the `Help` button in the web-app with content

## Install

We provide extensive instructions on our [installation](https://github.com/jpylypiw/easywall/blob/master/docs/INSTALL.md) page.
You can find a script for automatic downloading and installation.

## Documentation

Check the **[docs folder](https://github.com/jpylypiw/easywall/tree/master/docs)**.

## License

easywall is GNU General Public License v3.0.

## Screenshots

![Screenshot 1](https://i.imgur.com/eQAHOUc.png)
![Screenshot 2](https://i.imgur.com/N2cdm0h.png)
![Screenshot 3](https://i.imgur.com/pjtJuq5.png)
![Screenshot 4](https://i.imgur.com/SSTPaXO.png)
![Screenshot 5](https://i.imgur.com/EPHUjI3.png)
![Screenshot 6](https://i.imgur.com/X3sdFO3.png)
![Screenshot 7](https://i.imgur.com/5kd2Nql.png)
![Screenshot 8](https://i.imgur.com/jjZTxrV.png)
![Screenshot 9](https://i.imgur.com/owPACSx.png)
