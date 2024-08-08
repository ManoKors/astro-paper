---
author: Sat Naing
pubDatetime: 2024-08-08T10:00:00Z
title: How to Resolve "DNS Spoofing Detected" Error on macOS and Raspberry Pi
slug: resolve-dns-spoofing-error-macos-raspberry-pi
featured: true
draft: false
tags:
  - macOS
  - Raspberry Pi
  - SSH
  - Troubleshooting
description: Learn how to resolve the "DNS Spoofing Detected" error when using SSH on macOS to connect to a Raspberry Pi. This guide walks you through understanding the issue and how to fix it safely.
---

Encountering the "DNS Spoofing Detected" error when trying to SSH into your Raspberry Pi from macOS can be alarming, but it’s usually harmless and fixable. This guide will walk you through understanding and resolving this issue.

## Table of contents

## Understanding the "DNS Spoofing Detected" Error

When you see this error:

```plaintext
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@       WARNING: POSSIBLE DNS SPOOFING DETECTED!          @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
The ECDSA host key for pi.local has changed,
and the key for the corresponding IP address 2001:9e8:5abf:f000:2ecf:67ff:fe5b:4416
is unknown. This could either mean that
DNS SPOOFING is happening or the IP address for the host
and its host key have changed at the same time.
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@    WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!     @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!
Someone could be eavesdropping on you right now (man-in-the-middle attack)!
It is also possible that a host key has just been changed.
