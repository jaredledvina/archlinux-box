## How to use
1. Install Packer: https://www.packer.io/docs/install/index.html
2. Installed Vagrant: https://www.vagrantup.com/docs/installation/
3. `cd packer`
4. `packer build archlinux.json`
5. `cd ..`
6. `vagrant up`
7. `vagrant ssh`

To debug/step through the Packer build, use `packer build -debug archlinux.json`
