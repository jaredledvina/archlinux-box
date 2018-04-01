## How to use
1. Install Packer: https://www.packer.io/docs/install/index.html
2. Installed Vagrant: https://www.vagrantup.com/docs/installation/
3. `packer build packer/archlinux.json`
5. `vagrant up`
6. `vagrant ssh`

To debug/step through the Packer build, use ``packer build -debug archlinux.json``
