# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.define "ubuntu_mkdev" do |t|
  end

  config.vm.provider "virtualbox" do |v|
    v.name = "ubuntu_mkdev"
  end

  config.vm.network "private_network", ip: "10.110.0.10"
end


