---
author:
  name: Linode Community
  email: docs@linode.com
description: 'Caddy is a fast, cross-platform HTTP/2 web server with automatic HTTPS. This guide provides an introduction to installing Caddy on an Ubuntu 14.04 LTS server.'
keywords: 'Caddy,Ubuntu,web server,web hosting'
license: '[CC BY-ND 3.0](http://creativecommons.org/licenses/by-nd/3.0/us/)'
published: 'Weekday, Month 00th, 2015'
modified: Friday, January 1st, 2016
modified_by:
  name: Linode
title: 'Caddy Web Server on Ubuntu 14.04 LTS'
contributor:
  name: Zhan Tong Zhang
  link: https://github.com/zhantongz
external_resources:
  - '[Caddy User Guide](https://caddyserver.com/docs)'
---

*This is a Linode Community guide. Write for us and earn $250 per published guide.*
<hr>

[Caddy](https://caddyserver.com/) is a fast, cross-platform HTTP/2 web server with automatic HTTPS. This guide provides an introduction to installing Caddy on an Ubuntu 14.04 LTS server.

## Before You Begin

1.  Familiarize yourself with our [Getting Started](/docs/getting-started) guide and complete the steps for setting your Linode's hostname and timezone.

2.  This guide will use `sudo` wherever possible. Complete the sections of our [Securing Your Server](/docs/security/securing-your-server) to create a standard user account, harden SSH access and remove unnecessary network services. Do **not** follow the Configure a Firewall section yet--this guide includes firewall rules specifically for a Caddy server.

3.  Update your system.

        sudo apt-get update && sudo apt-get upgrade

{: .note}
>
>This guide is written for a non-root user. Commands that require elevated privileges are prefixed with `sudo`. If you’re not familiar with the `sudo` command, you can check our [Users and Groups](/docs/tools-reference/linux-users-and-groups) guide.

## Installing Caddy
Caddy is not available from the official repository, so you need to download it from its official website at https://caddyserver.com/download.
