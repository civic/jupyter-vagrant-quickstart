# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 8888, host: 8888
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get install -y git
    wget http://repo.continuum.io/archive/Anaconda3-4.0.0-Linux-x86_64.sh 
    sudo -u vagrant -H bash Anaconda3-4.0.0-Linux-x86_64.sh  -b
  SHELL
end
