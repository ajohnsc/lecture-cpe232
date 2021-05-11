# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define "centos0" do |centos|
    centos.vm.box = "centos/8"
    centos.vm.hostname = "centos0-vm"
    centos.vm.network "private_network", ip: "192.168.5.3", virtualbox_intnet: true
    
    centos.vm.provider "virtualbox" do |vb|
      vb.name = "centos0-vm"
      vb.cpus = 1
      vb.memory = 1024
    end
  end

  config.vm.define "ubuntu0" do |ubuntu|
    ubuntu.vm.box = "ubuntu/focal64"
    ubuntu.vm.hostname = "ubuntu1-vm"
    ubuntu.vm.network "private_network", ip: "192.168.5.2", virtualbox_intnet: true

    ubuntu.vm.provider "virtualbox" do |vb|
      vb.name = "ubuntu0-vm"
      vb.cpus = 1
      vb.memory = 1024
    end
  end

end
