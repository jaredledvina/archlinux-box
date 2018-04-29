## How to use
1. Install Packer: https://www.packer.io/docs/install/index.html
2. Installed Vagrant: https://www.vagrantup.com/docs/installation/
3. `cd packer`
4. `packer build -force archlinux.json`
5. `cd ..`
6. `vagrant up`
7. `vagrant ssh`

To debug/step through the Packer build, use `packer build -force -debug archlinux.json`
Alternatively, if you want to be prompted only on failures. use ` packer build -on-error=ask -force archlinux.json`

To force a full rebuild and reset Vagrant:
1. `rm -rf packer/{archlinux.box,archlinux.box.checksum,output-virtualbox-iso}`
2. `vagrant box remove --all --force archlinux-box`
3. Follow the build steps above
