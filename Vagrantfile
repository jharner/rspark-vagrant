# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "jharner/rspark"
  config.vm.box_check_update = true
  config.vm.network "forwarded_port", guest: 8787, host: 8787
  config.vm.provider "virtualbox" do |vb|
  	vb.memory = 2048
  end
end
