# libvirt-packer-scripts
Packer scripts for creating Libvirt/KVM boxes for Vagrant.

This repository holds Packer scripts for creating a Vagrant Box for
Ubuntu 16.04/Xenial (using Libvirt as a provider).

To build this box yourself, you need the following software:
- Vagrant
- Libvirt and QEMU
- The Vagrant-libvirt plugin
- Packer

My tool versions are:
- Vagrant 1.9.3
- Libvirt 1.2.18.2
- Vagrant-libvirt 0.37
- Packer 1.0.0

To build the Vagrant box, switch into the `ubuntu-16.04` directory and run
`packer build ubuntu-16.04-minimal.json`. Note that this will take awhile because
the packer script will try to download the Ubuntu ISO if it doesn't have it cached.
