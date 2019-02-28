# Commercium Masternode Setup

A step by step guide how to setup your Commercium Masternode on Windows/Linux/MacOS local wallet & Linux VPS as remote MN.

Choose one of the 2 available script options.

# Install script 1 #

Install script 1 will install the precompiled Commercium daemon

[part2_linux_vps_setup.sh](https://github.com/CommerciumBlockchain/masternode-scripts/blob/master/part2_linux_vps_setup.sh)

Visit:

https://medium.com/commercium-guides/how-to-set-up-a-commercium-masternode-da7361c2e47a 
Windows guide

https://medium.com/commercium-guides/how-to-set-up-a-commercium-masternode-in-linux-14d42e536dfb 
Linux guide

# Install script 2 #

Install script 2 will install the Commercium daemon with all dependencies from the source code

[install.sh]https://github.com/CommerciumBlockchain/masternode-scripts/blob/master/install.sh

## Features: ##

- Auto update to newer versions
- Auto daemon-check and restart if stuck
- Log file clearing
- Auto script check
- Runs commerciumd on startup
- Single/Multi MN install

> **This shell script has 4 cronjobs:**

1. [Check-scripts.sh](https://github.com/CommerciumBlockchain/masternode-scripts/blob/master/Masternode/Check-scripts.sh)
2. [daemon_check.sh](https://github.com/CommerciumBlockchain/masternode-scripts/blob/master/Masternode/daemon_check.sh)
3. [clearlog.sh](https://github.com/CommerciumBlockchain/masternode-scripts/blob/master/Masternode/clearlog.sh)
4. [UpdateNode.sh](https://github.com/CommerciumBlockchain/masternode-scripts/blob/master/Masternode/UpdateNode.sh)

As this script must be run as Root, make sure to secure your VPS with additional security measurements.

> **Version 1.0.1:**

Login to your vps as root, download and run the install.sh file using this command:

```
curl -O https://raw.githubusercontent.com/CommerciumBlockchain/masternode-scripts/master/install.sh > install.sh
bash install.sh
```

### Bash Checker for Masternodes on Ubuntu 16.04 LTS x64 <This script must be run as root user!>

------

```
curl -O https://raw.githubusercontent.com/CommerciumBlockchain/masternode-scripts/master/check-masternode.sh > check-masternode.sh
bash check-masternode.sh
```
