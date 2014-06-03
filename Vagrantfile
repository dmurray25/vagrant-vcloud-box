# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "box-cutter/ubuntu1404-desktop"

  config.vm.provision "shell", path: "scripts/install-git.sh"
  config.vm.provision "shell", path: "scripts/install-vagrant.sh"
  config.vm.provision "shell", path: "scripts/install-ssh-keys.sh", privileged: false
  config.vm.provision "shell", path: "scripts/install-vagrant-vcloud.sh", privileged: false
  config.vm.provision "shell", path: "scripts/install-vagrantfile.sh", privileged: false

end