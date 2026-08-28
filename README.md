# Awesome SSH with stars

> A curated list of *SSH* [apps](#apps), [libraries](#libraries) and [resources](#resources).

<h2 align="center"><img src="https://raw.githubusercontent.com/moul/awesome-ssh/master/logo.jpg" width="400" /></h2>

Inspired by the [awesome](https://github.com/sindresorhus/awesome) ⭐ 500,716 | 🐛 105 | 📅 2026-08-21 list thing.

Please read the [contribution guidelines](CONTRIBUTING.md) if you want to contribute.

**Check out my [blog](https://manfred.life/) 🦄 or say *hi* on [Twitter](https://twitter.com/moul).**

## Table of Contents

* [Apps](#apps)
  * [`.ssh/config`](#sshconfig)
  * [Tools using the *SSH* protocol](#tools-using-the-ssh-protocol)
  * [Servers](#servers)
  * [Network](#network)
  * [Multiplexers](#multiplexers)
  * [SSH Keys / Authentication](#ssh-keys--authentication)
  * [SSH agent](#ssh-agent)
  * [Tools](#tools)
  * [Automation](#automation)
  * [Web](#web)
  * [Testing / Honeypots](#testing--honeypots)
  * [Alternatives to SSH](#alternatives-to-ssh)
* [Libraries](#libraries)
* [Resources](#resources)
  * [Tutorials](#tutorials)
  * [Security](#security)
  * [Documentation](#documentation)
  * [Community](#community)

## Apps

### `.ssh/config`

* [storm](https://github.com/emre/storm) ⚠️ Archived [![stars](https://img.shields.io/github/stars/emre/storm.svg?style=social\&label=stars)](https://github.com/emre/storm) ⚠️ Archived - Manage your *SSH* like a boss.
* [`assh`](https://github.com/moul/assh) ⭐ 3,218 | 🐛 100 | 🌐 Go | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/moul/advanced-ssh-config.svg?style=social\&label=stars)](https://github.com/moul/advanced-ssh-config) ⭐ 3,218 | 🐛 100 | 🌐 Go | 📅 2026-08-28 - Transparent wrapper (ProxyCommand) that adds regex, aliases, gateways, includes, dynamic hostnames to *SSH* and `ssh-config`. *Previously: `advanced-ssh-config`*
* [ec2ssh](https://github.com/mirakui/ec2ssh) ⭐ 252 | 🐛 1 | 🌐 Ruby | 📅 2023-12-25 [![stars](https://img.shields.io/github/stars/mirakui/ec2ssh.svg?style=social\&label=stars)](https://github.com/mirakui/ec2ssh) ⭐ 252 | 🐛 1 | 🌐 Ruby | 📅 2023-12-25 - A `ssh_config` manager for *AWS EC2*.
* [ssh-config](https://github.com/dbrady/ssh-config) ⭐ 139 | 🐛 0 | 🌐 Ruby | 📅 2020-12-29 [![stars](https://img.shields.io/github/stars/dbrady/ssh-config.svg?style=social\&label=stars)](https://github.com/dbrady/ssh-config) ⭐ 139 | 🐛 0 | 🌐 Ruby | 📅 2020-12-29 - A tool to help manage your `.ssh/config` file.
* [ansible-ssh-config](https://github.com/gaqzi/ansible-ssh-config) ⚠️ Archived [![stars](https://img.shields.io/github/stars/gaqzi/ansible-ssh-config.svg?style=social\&label=stars)](https://github.com/gaqzi/ansible-ssh-config) ⚠️ Archived - Letting *Ansible* manage `ssh_config`.

### Tools using the *SSH* protocol

* [scp](http://linux.die.net/man/1/scp) - Secure remote file copy utility over *SSH*.
* [rsync](https://rsync.samba.org) - Fast incremental transfer utility that supports *SSH*.
* [sftp](https://en.wikipedia.org/wiki/SSH_File_Transfer_Protocol) - File transfer protocol over *SSH*.
* [curl](http://curl.haxx.se) - Command line tool and library to transfer data (support `sftp`).

### Servers

* [teleport](https://github.com/gravitational/teleport) ⭐ 20,856 | 🐛 3,335 | 🌐 Go | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/gravitational/teleport.svg?style=social\&label=stars)](https://github.com/gravitational/teleport) ⭐ 20,856 | 🐛 3,335 | 🌐 Go | 📅 2026-08-28 - Modern *SSH* server for clusters and teams.
* [ssh-chat](https://github.com/shazow/ssh-chat) ⭐ 5,910 | 🐛 54 | 🌐 Go | 📅 2026-01-10 [![stars](https://img.shields.io/github/stars/shazow/ssh-chat.svg?style=social\&label=stars)](https://github.com/shazow/ssh-chat) ⭐ 5,910 | 🐛 54 | 🌐 Go | 📅 2026-01-10 - Chat over *SSH*.
* [whosthere](https://github.com/FiloSottile/whosthere) ⭐ 2,361 | 🐛 10 | 🌐 Go | 📅 2026-04-16 [![stars](https://img.shields.io/github/stars/FiloSottile/whosthere.svg?style=social\&label=stars)](https://github.com/FiloSottile/whosthere) ⭐ 2,361 | 🐛 10 | 🌐 Go | 📅 2026-04-16 - A *SSH* server that knows who you are. `$ ssh whoami.filippo.io`.
* [ShellHub](https://github.com/shellhub-io/shellhub) ⭐ 2,063 | 🐛 25 | 🌐 TypeScript | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/shellhub-io/shellhub.svg?style=social\&label=stars)](https://github.com/shellhub-io/shellhub) ⭐ 2,063 | 🐛 25 | 🌐 TypeScript | 📅 2026-08-28 - A *SSH* gateway for remotely accessing any Linux device behind firewall and NAT.
* [sshportal](https://github.com/moul/sshportal) ⭐ 1,940 | 🐛 81 | 🌐 Go | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/moul/sshportal.svg?style=social\&label=stars)](https://github.com/moul/sshportal) ⭐ 1,940 | 🐛 81 | 🌐 Go | 📅 2026-08-28 - simple, fun, and transparent SSH (& Telnet) Bastion Server
* [sshmuxd](https://github.com/joushou/sshmuxd) ⚠️ Archived [![stars](https://img.shields.io/github/stars/joushou/sshmuxd.svg?style=social\&label=stars)](https://github.com/joushou/sshmuxd) ⚠️ Archived - `sshmux` frontend.
* [sshcommand](https://github.com/dokku/sshcommand) ⭐ 388 | 🐛 0 | 🌐 Shell | 📅 2026-08-27 [![stars](https://img.shields.io/github/stars/dokku/sshcommand.svg?style=social\&label=stars)](https://github.com/dokku/sshcommand) ⭐ 388 | 🐛 0 | 🌐 Shell | 📅 2026-08-27 - Turn *SSH* into a thin client specifically for your app.
* [x84](https://github.com/jquast/x84) ⚠️ Archived [![stars](https://img.shields.io/github/stars/jquast/x84.svg?style=social\&label=stars)](https://github.com/jquast/x84) ⚠️ Archived - A *python* `telnet`/`ssh` server for modern *UTF-8* and classic *cp437* network virtual terminals. In spirit of classic software such as *ami/x*, *teleguard*, *renegade*, *iniquity*.
* [sshfront](https://github.com/gliderlabs/sshfront) ⭐ 328 | 🐛 4 | 🌐 Go | 📅 2023-12-15 [![stars](https://img.shields.io/github/stars/gliderlabs/sshfront.svg?style=social\&label=stars)](https://github.com/gliderlabs/sshfront) ⭐ 328 | 🐛 4 | 🌐 Go | 📅 2023-12-15 - Programmable *SSH* frontend.
* [ssh2docker](https://github.com/moul/ssh2docker) ⭐ 198 | 🐛 24 | 🌐 Go | 📅 2026-08-19 [![stars](https://img.shields.io/github/stars/moul/ssh2docker.svg?style=social\&label=stars)](https://github.com/moul/ssh2docker) ⭐ 198 | 🐛 24 | 🌐 Go | 📅 2026-08-19 - *SSH* server to Docker containers.
* [ssh-proxy](https://github.com/ml-tooling/ssh-proxy) ⭐ 87 | 🐛 1 | 🌐 Python | 📅 2020-08-04 [![stars](https://img.shields.io/github/stars/ml-tooling/ssh-proxy.svg?style=social\&label=stars)](https://github.com/ml-tooling/ssh-proxy) ⭐ 87 | 🐛 1 | 🌐 Python | 📅 2020-08-04 - Dockerized SSH bastion to proxy SSH connections to arbitrary containers.

### Network

* [ngrok](https://github.com/inconshreveable/ngrok) ⚠️ Archived [![stars](https://img.shields.io/github/stars/inconshreveable/ngrok.svg?style=social\&label=stars)](https://github.com/inconshreveable/ngrok) ⚠️ Archived - Introspected tunnels to localhost.
* [sshuttle](https://github.com/sshuttle/sshuttle) ⭐ 13,532 | 🐛 212 | 🌐 Python | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/sshuttle/sshuttle.svg?style=social\&label=stars)](https://github.com/sshuttle/sshuttle) ⭐ 13,532 | 🐛 212 | 🌐 Python | 📅 2026-08-28 - Transparent proxy server that works as a poor man's *VPN*. Forwards over `ssh`. Doesn't require admin. Works with *Linux* and *MacOS*. Supports *DNS tunneling*.
* [sshfs](https://github.com/libfuse/sshfs) ⭐ 7,639 | 🐛 62 | 🌐 C | 📅 2026-08-08 [![stars](https://img.shields.io/github/stars/libfuse/sshfs.svg?style=social\&label=stars)](https://github.com/libfuse/sshfs) ⭐ 7,639 | 🐛 62 | 🌐 C | 📅 2026-08-08 - Filesystem client based on the *SSH* File Transfer Protocol.
* [sslh](https://github.com/yrutschle/sslh) ⭐ 5,109 | 🐛 47 | 🌐 C | 📅 2026-08-20 [![stars](https://img.shields.io/github/stars/yrutschle/sslh.svg?style=social\&label=stars)](https://github.com/yrutschle/sslh) ⭐ 5,109 | 🐛 47 | 🌐 C | 📅 2026-08-20 - Applicative Protocol Multiplexer (i.e: *SSH* + *HTTPS*).
* [localtunnel](https://github.com/progrium/localtunnel) ⭐ 3,227 | 🐛 13 | 🌐 Go | 📅 2022-05-17 [![stars](https://img.shields.io/github/stars/progrium/localtunnel.svg?style=social\&label=stars)](https://github.com/progrium/localtunnel) ⭐ 3,227 | 🐛 13 | 🌐 Go | 📅 2022-05-17 - Expose localhost servers to the Internet.
* [wssh](https://github.com/aluzzardi/wssh) ⭐ 1,371 | 🐛 26 | 🌐 JavaScript | 📅 2019-02-12 [![stars](https://img.shields.io/github/stars/aluzzardi/wssh.svg?style=social\&label=stars)](https://github.com/aluzzardi/wssh) ⭐ 1,371 | 🐛 26 | 🌐 JavaScript | 📅 2019-02-12 - *SSH* to WebSockets Bridge.
* [sshpiper](https://github.com/tg123/sshpiper) ⭐ 1,304 | 🐛 21 | 🌐 Go | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/tg123/sshpiper.svg?style=social\&label=stars)](https://github.com/tg123/sshpiper) ⭐ 1,304 | 🐛 21 | 🌐 Go | 📅 2026-08-28 - The missing reverse proxy for ssh scp.
* [switcher](https://github.com/jamescun/switcher) ⭐ 903 | 🐛 4 | 🌐 Go | 📅 2019-03-15 [![stars](https://img.shields.io/github/stars/jamescun/switcher.svg?style=social\&label=stars)](https://github.com/jamescun/switcher) ⭐ 903 | 🐛 4 | 🌐 Go | 📅 2019-03-15 - Run *SSH* and *HTTP(S)* on the same port.
* [sshttp](https://github.com/stealth/sshttp) ⭐ 893 | 🐛 2 | 🌐 C++ | 📅 2023-06-22 [![stars](https://img.shields.io/github/stars/stealth/sshttp.svg?style=social\&label=stars)](https://github.com/stealth/sshttp) ⭐ 893 | 🐛 2 | 🌐 C++ | 📅 2023-06-22 - *SSH*/*HTTP(S)* multiplexer. Run a webserver and a `sshd` on the same port w/o changes.
* [quicssh](https://github.com/moul/quicssh) ⭐ 860 | 🐛 22 | 🌐 Go | 📅 2026-08-19 [![stars](https://img.shields.io/github/stars/moul/quicssh.svg?style=social\&label=stars)](https://github.com/moul/quicssh) ⭐ 860 | 🐛 22 | 🌐 Go | 📅 2026-08-19 - QUIC proxy for SSH
* [docker-volume-sshfs](https://github.com/vieux/docker-volume-sshfs) ⚠️ Archived [![stars](https://img.shields.io/github/stars/vieux/docker-volume-sshfs.svg?style=social\&label=stars)](https://github.com/vieux/docker-volume-sshfs) ⚠️ Archived - `sshfs` docker volume plugin.
* [tund](https://github.com/aphyr/tund) ⭐ 418 | 🐛 1 | 🌐 Ruby | 📅 2020-02-07 [![stars](https://img.shields.io/github/stars/aphyr/tund.svg?style=social\&label=stars)](https://github.com/aphyr/tund) ⭐ 418 | 🐛 1 | 🌐 Ruby | 📅 2020-02-07 - *SSH* reverse tunnel daemon.
* [Mosh](https://mosh.mit.edu) - The mobile shell.
* [autossh](http://www.harding.motd.ca/autossh/) - Automatically respawn *SSH* session after network interruption.
* [sshhub](https://sshhub.de) - Web Service: access your SSH servers behind firewalls (ssh-teamviewer).

### Multiplexers

* [clusterssh](https://github.com/duncs/clusterssh) ⭐ 988 | 🐛 28 | 🌐 Perl | 📅 2026-04-28 [![stars](https://img.shields.io/github/stars/duncs/clusterssh.svg?style=social\&label=stars)](https://github.com/duncs/clusterssh) ⭐ 988 | 🐛 28 | 🌐 Perl | 📅 2026-04-28 - Cluster admin via *SSH*.
* [i2cssh](https://github.com/wouterdebie/i2cssh) ⭐ 569 | 🐛 3 | 🌐 Python | 📅 2025-11-04 [![stars](https://img.shields.io/github/stars/wouterdebie/i2cssh.svg?style=social\&label=stars)](https://github.com/wouterdebie/i2cssh) ⭐ 569 | 🐛 3 | 🌐 Python | 📅 2025-11-04 - `csshX` like *SSH* tool for *iTerm2*.
* [tm](https://github.com/Ganneff/tm) ⚠️ Archived [![stars](https://img.shields.io/github/stars/Ganneff/tm.svg?style=social\&label=stars)](https://github.com/Ganneff/tm) ⚠️ Archived - `tmux` manager / helper.
* [tmux](https://tmux.github.io) - Terminal multiplexer.
* [tmux-cssh](https://github.com/dennishafemann/tmux-cssh) [![stars](https://img.shields.io/github/stars/dennishafemann/tmux-cssh.svg?style=social\&label=stars)](https://github.com/dennishafemann/tmux-cssh) - `tmux` with a *ClusterSSH*-like behavior.
* [ClusterSSH](http://sourceforge.net/projects/clusterssh/) - Controls a number of `xterm` windows via a single graphical console.

### *SSH* keys / Authentication

* [kr](https://github.com/KryptCo/kr) ⚠️ Archived [![stars](https://img.shields.io/github/stars/dolmen/github-keygen.svg?style=social\&label=stars)](https://github.com/KryptCo/kr) ⚠️ Archived - Kr agent that route access request to the paired mobile phone where Kryptonite is installed.
* [totp-ssh-fluxer](https://github.com/benjojo/totp-ssh-fluxer) ⭐ 947 | 🐛 2 | 🌐 Go | 📅 2022-08-31 [![stars](https://img.shields.io/github/stars/benjojo/totp-ssh-fluxer.svg?style=social\&label=stars)](https://github.com/benjojo/totp-ssh-fluxer) ⭐ 947 | 🐛 2 | 🌐 Go | 📅 2022-08-31 - A way to make sure your `sshd` port changes every 30 seconds.
* [authy-ssh](https://github.com/authy/authy-ssh) ⚠️ Archived [![stars](https://img.shields.io/github/stars/authy/authy-ssh.svg?style=social\&label=stars)](https://github.com/authy/authy-ssh) ⚠️ Archived - Easy *two-factor* authentication for *SSH* servers.
* [github-auth](https://github.com/chrishunt/github-auth) ⭐ 390 | 🐛 3 | 🌐 Ruby | 📅 2018-08-27 [![stars](https://img.shields.io/github/stars/chrishunt/github-auth.svg?style=social\&label=stars)](https://github.com/chrishunt/github-auth) ⭐ 390 | 🐛 3 | 🌐 Ruby | 📅 2018-08-27 - *SSH* key management for GitHub users.
* [HIBA](https://github.com/google/hiba) ⚠️ Archived [![stars](https://img.shields.io/github/stars/google/hiba.svg?style=social\&label=stars)](https://github.com/google/hiba) ⚠️ Archived - Central management of access to a fleet of machines without pushing authorized\_users files.
* [github-keygen](https://github.com/dolmen/github-keygen) ⭐ 271 | 🐛 25 | 🌐 Perl | 📅 2026-07-27 [![stars](https://img.shields.io/github/stars/dolmen/github-keygen.svg?style=social\&label=stars)](https://github.com/dolmen/github-keygen) ⭐ 271 | 🐛 25 | 🌐 Perl | 📅 2026-07-27 - Easy creation of secure *SSH* configuration for your GitHub account(s).
* [cipherhub](https://github.com/substack/cipherhub) [![stars](https://img.shields.io/github/stars/substack/cipherhub.svg?style=social\&label=stars)](https://github.com/substack/cipherhub) - Encrypt messages based on *SSH* public keys with easy import from GitHub.
* [Slack notifications](http://www.ryanbrink.com/slack-ssh-session-notifications/) ([archived version](https://web.archive.org/web/20160505202303/http://www.ryanbrink.com/slack-ssh-session-notifications/)) - Guide to setup Slack notifications (can be modified for other services).
* [ServerAuth](https://serverauth.com) - Automatically sync SSH access across servers

### *SSH* agent

* [oh-my-zsh/plugins/ssh-agent](https://github.com/robbyrussell/oh-my-zsh) ⭐ 189,420 | 🐛 578 | 🌐 Shell | 📅 2026-08-25 [![stars](https://img.shields.io/github/stars/robbyrussell/oh-my-zsh.svg?style=social\&label=stars)](https://github.com/robbyrussell/oh-my-zsh) ⭐ 189,420 | 🐛 578 | 🌐 Shell | 📅 2026-08-25 - `ssh-agent` plugin for `zsh`.
* [ssh-ident](https://github.com/ccontavalli/ssh-ident) ⭐ 985 | 🐛 33 | 🌐 Python | 📅 2022-01-08 [![stars](https://img.shields.io/github/stars/ccontavalli/ssh-ident.svg?style=social\&label=stars)](https://github.com/ccontavalli/ssh-ident) ⭐ 985 | 🐛 33 | 🌐 Python | 📅 2022-01-08 - Different agents and different keys for different projects, with `ssh`.
* [sshecret](https://github.com/thcipriani/sshecret) ⭐ 72 | 🐛 2 | 🌐 Python | 📅 2024-01-05 - Automatically create and manage multiple agents for multiple keys.

### Tools

* [xxh](https://github.com/xxh/xxh) ⭐ 6,077 | 🐛 30 | 🌐 Python | 📅 2026-06-02 [![stars](https://img.shields.io/github/stars/xxh/xxh.svg?style=social\&label=stars)](https://github.com/xxh/xxh) ⭐ 6,077 | 🐛 30 | 🌐 Python | 📅 2026-06-02 - Bring your favorite shell wherever you go through the ssh.
* [ssh-ping](https://github.com/vaporup/ssh-tools) ⚠️ Archived [![stars](https://img.shields.io/github/stars/vaporup/ssh-tools.svg?style=social\&label=stars)](https://github.com/vaporup/ssh-tools) ⚠️ Archived - check if host is reachable using ssh\_config
* [ssh-vault](https://github.com/ssh-vault/ssh-vault) ⭐ 508 | 🐛 1 | 🌐 Rust | 📅 2026-08-24 [![stars](https://img.shields.io/github/stars/ssh-vault/ssh-vault.svg?style=social\&label=stars)](https://github.com/ssh-vault/ssh-vault) ⭐ 508 | 🐛 1 | 🌐 Rust | 📅 2026-08-24 - encrypt/decrypt files using ssh keys
* [SSHPry v2](https://github.com/nopernik/SSHPry2.0) ⭐ 400 | 🐛 2 | 🌐 Python | 📅 2017-10-12 [![stars](https://img.shields.io/github/stars/nopernik/SSHPry2.0.svg?style=social\&label=stars)](https://github.com/nopernik/SSHPry2.0) ⭐ 400 | 🐛 2 | 🌐 Python | 📅 2017-10-12 - Spy & Control os SSH Connected client's TTY
* [kyrat](https://github.com/fsquillace/kyrat) ⭐ 282 | 🐛 9 | 🌐 Shell | 📅 2023-05-02 [![stars](https://img.shields.io/github/stars/fsquillace/kyrat.svg?style=social\&label=stars)](https://github.com/fsquillace/kyrat) ⭐ 282 | 🐛 9 | 🌐 Shell | 📅 2023-05-02 - SSH wrapper script that brings your dotfiles always with you on Linux and OSX.
* [redial](https://github.com/taypo/redial) ⭐ 206 | 🐛 12 | 🌐 Python | 📅 2026-01-18 [![stars](https://img.shields.io/github/stars/taypo/redial?style=social)](https://github.com/taypo/redial) ⭐ 206 | 🐛 12 | 🌐 Python | 📅 2026-01-18 - Terminal Based SSH Session Manager for Unix Systems
* [sshrc](https://github.com/danrabinowitz/sshrc) ⭐ 104 | 🐛 0 | 📅 2014-09-15 [![stars](https://img.shields.io/github/stars/danrabinowitz/sshrc.svg?style=social\&label=stars)](https://github.com/danrabinowitz/sshrc) ⭐ 104 | 🐛 0 | 📅 2014-09-15 - Bring your `.bashrc`, `.vimrc`, etc. with you when you `ssh`.

### Automation

* [Ansible](https://github.com/ansible/ansible) ⭐ 70,487 | 🐛 833 | 🌐 Python | 📅 2026-08-27 [![stars](https://img.shields.io/github/stars/ansible/ansible.svg?style=social\&label=stars)](https://github.com/ansible/ansible) ⭐ 70,487 | 🐛 833 | 🌐 Python | 📅 2026-08-27 - App deployment, configuration management and orchestration over *SSH*.
* [rtop](https://github.com/rapidloop/rtop) ⭐ 2,187 | 🐛 23 | 🌐 Go | 📅 2022-06-06 [![stars](https://img.shields.io/github/stars/rapidloop/rtop.svg?style=social\&label=stars)](https://github.com/rapidloop/rtop) ⭐ 2,187 | 🐛 23 | 🌐 Go | 📅 2022-06-06 - Interactive, remote system monitoring tool based on *SSH*.
* [parallel-ssh](https://github.com/ParallelSSH/parallel-ssh) ⭐ 1,282 | 🐛 10 | 🌐 Python | 📅 2026-08-05 [![stars](https://img.shields.io/github/stars/ParallelSSH/parallel-ssh.svg?style=social\&label=stars)](https://github.com/ParallelSSH/parallel-ssh) ⭐ 1,282 | 🐛 10 | 🌐 Python | 📅 2026-08-05 - Provides parallel versions of OpenSSH and related tools.
* [DSH - Dancer's shell / distributed shell](https://www.netfort.gr.jp/~dancer/software/dsh.html.en) - Wrapper for executing multiple remote shell commands from one command line.
* [SSH Power Tool](https://code.google.com/p/sshpt/) - Execute commands and upload files to many servers simultaneously without using pre-shared keys.

### Web

* [GateOne](https://github.com/liftoff/GateOne) ⭐ 6,298 | 🐛 365 | 🌐 JavaScript | 📅 2023-03-17 [![stars](https://img.shields.io/github/stars/liftoff/GateOne.svg?style=social\&label=stars)](https://github.com/liftoff/GateOne) ⭐ 6,298 | 🐛 365 | 🌐 JavaScript | 📅 2023-03-17 - HTML5-powered terminal emulator and *SSH* client.
* [KeyBox](https://github.com/skavanagh/KeyBox) ⭐ 3,541 | 🐛 130 | 🌐 Java | 📅 2026-08-28 [![stars](https://img.shields.io/github/stars/skavanagh/KeyBox.svg?style=social\&label=stars)](https://github.com/skavanagh/KeyBox) ⭐ 3,541 | 🐛 130 | 🌐 Java | 📅 2026-08-28 - Web-based *SSH* console that centrally manages administrative access to systems.
* [SSHmon](https://github.com/hpello/sshmon) ⭐ 206 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-11 [![stars](https://img.shields.io/github/stars/hpello/sshmon.svg?style=social\&label=stars)](https://github.com/hpello/sshmon) ⭐ 206 | 🐛 1 | 🌐 TypeScript | 📅 2026-08-11 - Real-time GUI to monitor SSH connections and establish port forwardings.
* [Secure Shell chrome extension](https://chrome.google.com/webstore/detail/secure-shell/pnhechapfaindjhompbnflcldabbghjo?hl=en)
* [Apache Guacamole](https://guacamole.incubator.apache.org/) - Apache Guacamole is a HTML5 based clientless remote desktop gateway. It supports standard protocols like VNC, RDP, and SSH.

### Testing / Honeypots

* [cowrie](https://github.com/micheloosterhof/cowrie) ⭐ 6,508 | 🐛 118 | 🌐 Python | 📅 2026-08-27 [![stars](https://img.shields.io/github/stars/micheloosterhof/cowrie.svg?style=social\&label=stars)](https://github.com/micheloosterhof/cowrie) ⭐ 6,508 | 🐛 118 | 🌐 Python | 📅 2026-08-27 - *SSH* Honeypot (based on kippo).
* [ssh-audit](https://github.com/arthepsy/ssh-audit) ⭐ 2,995 | 🐛 31 | 🌐 Python | 📅 2024-06-28 [![stars](https://img.shields.io/github/stars/arthepsy/ssh-audit.svg?style=social\&label=stars)](https://github.com/arthepsy/ssh-audit) ⭐ 2,995 | 🐛 31 | 🌐 Python | 📅 2024-06-28 - A tool for *SSH* server auditing.
* [sshesame](https://github.com/jaksi/sshesame) ⭐ 1,741 | 🐛 17 | 🌐 Go | 📅 2024-10-21 [![stars](https://img.shields.io/github/stars/jaksi/sshesame.svg?style=social\&label=stars)](https://github.com/jaksi/sshesame) ⭐ 1,741 | 🐛 17 | 🌐 Go | 📅 2024-10-21 - A fake SSH server that lets everyone in and logs their activity.
* [kippo](https://github.com/desaster/kippo) ⭐ 1,715 | 🐛 83 | 🌐 Python | 📅 2023-11-19 [![stars](https://img.shields.io/github/stars/desaster/kippo.svg?style=social\&label=stars)](https://github.com/desaster/kippo) ⭐ 1,715 | 🐛 83 | 🌐 Python | 📅 2023-11-19 - *SSH* Honeypot.
* [ssh-hammer](https://github.com/shazow/ssh-hammer) ⭐ 15 | 🐛 1 | 🌐 Go | 📅 2021-10-11 [![stars](https://img.shields.io/github/stars/shazow/ssh-hammer.svg?style=social\&label=stars)](https://github.com/shazow/ssh-hammer) ⭐ 15 | 🐛 1 | 🌐 Go | 📅 2021-10-11 - *SSH* load testing tool.
* [sshmitm](http://linux.die.net/man/8/sshmitm) - *SSH* monkey-in-the-middle.

### Alternatives to *SSH*

* [GoTTY](https://github.com/yudai/gotty) ⭐ 19,547 | 🐛 158 | 🌐 Go | 📅 2024-08-01 [![stars](https://img.shields.io/github/stars/yudai/gotty.svg?style=social\&label=stars)](https://github.com/yudai/gotty) ⭐ 19,547 | 🐛 158 | 🌐 Go | 📅 2024-08-01 - Share your terminal as web application.
* [ttyd](https://github.com/tsl0922/ttyd) ⭐ 12,273 | 🐛 113 | 🌐 C | 📅 2026-08-12 [![stars](https://img.shields.io/github/stars/tsl0922/ttyd.svg?style=social\&label=stars)](https://github.com/tsl0922/ttyd) ⭐ 12,273 | 🐛 113 | 🌐 C | 📅 2026-08-12 - Share your terminal over the web.
* [telnet](http://www.telnet.org/htm/faq.htm) - An unencrypted network protocol and an application used to connect to remote computers and issue commands.
* [rsh](https://en.wikipedia.org/wiki/Remote_Shell) - An unencrypted network protocol and application used to connect to remote computers and issue commands.

## Libraries

* C/C++
  * [libssh](https://www.libssh.org) - The *SSH* library.
* Golang
  * [sftp](https://github.com/pkg/sftp) ⭐ 1,664 | 🐛 60 | 🌐 Go | 📅 2026-07-22 [![stars](https://img.shields.io/github/stars/pkg/sftp.svg?style=social\&label=stars)](https://github.com/pkg/sftp) ⭐ 1,664 | 🐛 60 | 🌐 Go | 📅 2026-07-22 - *SFTP* support for the go.crypto/ssh package.
  * [Socker](https://github.com/cosiner/socker) ⭐ 252 | 🐛 1 | 🌐 Go | 📅 2023-03-29 [![stars](https://img.shields.io/github/stars/cosiner/socker.svg?style=social\&label=stars)](https://github.com/cosiner/socker) ⭐ 252 | 🐛 1 | 🌐 Go | 📅 2023-03-29 - Library for Go to simplify the use of *SSH*.
  * [go-sshkit](https://github.com/shazow/go-sshkit) ⭐ 23 | 🐛 1 | 🌐 Go | 📅 2015-12-28 [![stars](https://img.shields.io/github/stars/shazow/go-sshkit.svg?style=social\&label=stars)](https://github.com/shazow/go-sshkit) ⭐ 23 | 🐛 1 | 🌐 Go | 📅 2015-12-28 - Toolkit for building *SSH* servers and clients in Go.
  * [go-sshkeys](https://github.com/moul/go-sshkeys) ⭐ 5 | 🐛 1 | 🌐 Go | 📅 2023-12-01 - Golang SSH Keys manipulation library
  * [crypto/ssh](https://godoc.org/golang.org/x/crypto/ssh) - Built-in *SSH* client and server library.
* Java
  * [jsch](http://www.jcraft.com/jsch/) - Pure *java*, *BSD* licensed, *SSH2* client library.
* Javascript/Node.js
  * [ssh2](https://github.com/mscdex/ssh2) ⭐ 5,818 | 🐛 103 | 🌐 JavaScript | 📅 2026-08-20 [![stars](https://img.shields.io/github/stars/mscdex/ssh2.svg?style=social\&label=stars)](https://github.com/mscdex/ssh2) ⭐ 5,818 | 🐛 103 | 🌐 JavaScript | 📅 2026-08-20 - *SSH2* client and server modules written in pure *JavaScript* for *node.js*.
* Python
  * [paramiko](https://github.com/paramiko/paramiko) ⭐ 9,841 | 🐛 1,196 | 🌐 Python | 📅 2026-05-09 [![stars](https://img.shields.io/github/stars/paramiko/paramiko.svg?style=social\&label=stars)](https://github.com/paramiko/paramiko) ⭐ 9,841 | 🐛 1,196 | 🌐 Python | 📅 2026-05-09 - Native *Python* *SSHv2* protocol library.
* Ruby
  * [net-ssh](https://github.com/net-ssh/net-ssh) ⭐ 1,022 | 🐛 120 | 🌐 Ruby | 📅 2026-08-09 [![stars](https://img.shields.io/github/stars/net-ssh/net-ssh.svg?style=social\&label=stars)](https://github.com/net-ssh/net-ssh) ⭐ 1,022 | 🐛 120 | 🌐 Ruby | 📅 2026-08-09 - Pure *Ruby* implementation of an *SSH* (protocol 2) client.

## Resources

### Tutorials

* [How to use *SSH* to Connect to a Remote Server](https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-in-ubuntu)
* [Best practices](https://blog.0xbadc0de.be/archives/300)
* [Granting Temporary Access to Your Servers (Using Signed *SSH* Keys)](http://linux-audit.com/granting-temporary-access-to-servers-using-signed-ssh-keys/)
* [How to SSH login without a password](https://www.rosehosting.com/blog/ssh-login-without-password-using-ssh-keys/)
* [Gist: SSH Recipes](https://gist.github.com/mjalajel/beaa91a5f8d04ebb464c2c28da01406a) - Collection of recipes for writing awesome ssh config files.

### Security

* [01/14/2016](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2016-0777) - Integer Overflow `CVE 2016 077[7-8]`.
* [Security/Guidelines/OpenSSH - MozillaWiki](https://wiki.mozilla.org/Security/Guidelines/OpenSSH) - `sshd\_config` for `6.7+`, `5.3`.
* [Applied-Crypto-Hardening](https://github.com/BetterCrypto/Applied-Crypto-Hardening) ⭐ 701 | 🐛 120 | 🌐 TeX | 📅 2022-01-23 [![stars](https://img.shields.io/github/stars/BetterCrypto/Applied-Crypto-Hardening.svg?style=social\&label=stars)](https://github.com/BetterCrypto/Applied-Crypto-Hardening) ⭐ 701 | 🐛 120 | 🌐 TeX | 📅 2022-01-23 - `sshd\_config` for `6.X`

### Documentation

* [man page](http://linux.die.net/man/1/ssh)
* [Specifications (OpenSSH)](http://www.openssh.com/specs.html)
* [Wikipedia article](https://en.wikipedia.org/wiki/Secure_Shell)

### Community

* [StackOverflow](http://stackoverflow.com/questions/tagged/ssh)
* [ServerFault](http://serverfault.com/questions/tagged/ssh)

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Manfred Touron](https://github.com/moul) has waived all copyright and related or neighboring rights to this work.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-28._
