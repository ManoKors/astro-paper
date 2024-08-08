---
author: Mano Kors
pubDatetime: 2024-08-08T10:00:00Z
title: How to Docker on macOS and Raspberry Pi 5
slug: installing-docker-on-raspberry-pi-5
featured: true
draft: false
tags:
  - macOS
  - Raspberry Pi
  - Docker
  - How-To
description: Learn how to resolve the "DNS Spoofing Detected" error when using SSH on macOS to connect to a Raspberry Pi. This guide walks you through understanding the issue and how to fix it safely.
---

The first thing you want to do is to uninstall all conflicting packages that might be on the Raspberry Pi. Run the following command in side the Terminal after having made a SSH Connection with the Raspberry Pi.

```plaintext
for pkg in docker.io docker-doc docker-compose docker-compose-v2 podman-docker containerd runc; do sudo apt-get remove $pkg; done
```


The Output looks like this:

```plaintext
mano@pi:~$ for pkg in docker.io docker-doc docker-compose docker-compose-v2 podman-docker containerd runc; do sudo apt-get remove $pkg; done
[sudo] password for mano: 
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'docker.io' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'docker-doc' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'docker-compose' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'docker-compose-v2' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'podman-docker' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'containerd' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Package 'runc' is not installed, so not removed
0 upgraded, 0 newly installed, 0 to remove and 94 not upgraded.
````
