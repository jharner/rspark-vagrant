# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
  config.ssh.insert_key = false
  config.vm.box = "jharner/rspark"
  config.vm.box_check_update = true  
  config.vm.network "forwarded_port", guest: 8787, host: 8787
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--uartmode1", "disconnected"]
    vb.customize ["modifyvm", :id, "--memory", 4096]
    vb.name = "rspark"
  end

end
