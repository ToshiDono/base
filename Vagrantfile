# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.define "ubuntu_mkdev" do |t|
    t.vm.network "private_network", ip: "192.168.50.4"
  end

  config.vm.provider "virtualbox" do |v|
    v.name = "ubuntu_mkdev"
  end
  config.vm.provision "file", source: "~/.ssh/mac_ondoc.pub", destination: "~vagrant/.ssh/authorized_keys"
end
