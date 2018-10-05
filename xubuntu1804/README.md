# xubuntu1804

This directory contains build recipe for Xubuntu 18.04 based desktop [Vagrant](https://www.vagrantup.com/) box.

## Building the box

The default target of the `Makefile` builds and packages the Vagrant box.

## Details about the build

The `Vagrantfile` takes [`generic/ubuntu1804`](https://app.vagrantup.com/generic/boxes/ubuntu1804) box as base and
- applies the latest updates
- adds [virtualbox-guest-utils](https://packages.ubuntu.com/bionic/virtualbox-guest-utils)
- installs the XFCE desktop environment
- [cleans up and minimizes the VM for packaging](https://gist.github.com/carlessanagustin/2fb92e88f2068300a2ed)
- shuts down the VM
