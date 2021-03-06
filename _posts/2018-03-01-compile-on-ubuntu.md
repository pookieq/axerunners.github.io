---
layout: post
title: "How to compile AXE core on Ubuntu 16"
date: 2018-03-01
excerpt: "v1.1.1"
tags: [core, linux, guide]
comments: true
---

### Prepare the system

Update operating system and install dependencies

```
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git python-virtualenv virtualenv fail2ban
sudo apt-get install ufw
sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
sudo apt-get install libboost-all-dev
sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install libdb4.8-dev libdb4.8++-dev
sudo apt-get install libminiupnpc-dev libzmq3-dev
```

### Install AXE core and launch the client

Use following command to install AXE core

```
wget https://gist.github.com/charlesrocket/f5331e54b47344b6957781bbbea8dc33/raw/34bdba7c2b6dff507af43d544fee1e8d51ad69b4/axecore.sh && bash axecore.sh
```

Start GUI client with `axe-qt` or headless version with `axed`
