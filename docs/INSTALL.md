# How to Install easywall

You just need three simple steps for installing easywall on your system.

## Index

1. [Check Requirements](#require)
2. [Download and Install easywall](#easywall)

## 1. Check Requirements

- ssh (root access) on the server
- Currently we only support Debian based Servers

## 2. Download and Install easywall

```sh
cd /usr/local
git clone https://github.com/jpylypiw/easywall.git
cd easywall
```

You can **clone** the repository to get the **latest version** of easywall. You also can **download** the repository from GitHub and **unzip** it on your system.
We suggest to use the directories **/usr/local** or **/opt** for easywall Installation.

```sh
sudo chmod +x install.sh
sudo -H bash install.sh
```

We suggest to use the installer for proper installation. **You have to execute the installer as root user!** For manual installation execute the steps in the installer file on your own.
