# XLSForm Server

This repo lets developers setup an XLSForm server for testing. 

This server will appear like any other machine on your network. This allows you to connect external devices to test the server. We assume your network hands out IP addresses over DHCP. You can change this behavior in `Vagrantfile`.

Please don't use this server in production. It is not configured to be robust or safe.

## Install requirements
1. Install [ansible](https://docs.ansible.com/ansible/intro_installation.html) v2.3.1.0 or later.
1. Install [vagrant](https://www.vagrantup.com/docs/installation) v1.9.5 or later.
	1. Optional: Install [vagrant-cachier](https://github.com/fgrehm/vagrant-cachier) for faster builds.
1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) v5.1.22 or later.

## Provision and configure server
1. Clone this repository.
1. Run `vagrant up`.
1. After the server is provisioned, the server will be at [192.168.255.10](http://192.168.255.10)

## TODOs

1. Replace czue repo with odk repo after PRs are merged
1. gunicorn needs to be killed/restarted manually for config changes to take effect
