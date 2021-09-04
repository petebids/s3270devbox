# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-20.04"
  # add custom install stuff here 
  # see more complex example https://dev.to/vumdao/create-an-ubuntu-20-04-server-using-vagrant-3d2i
  config.vm.provision "shell", inline: <<-SHELL
  apt update
  apt install -y s3270
 SHELL

  config.vm.provider "virtualbox" do |vb|
   # Display the VirtualBox GUI when booting the machine
    vb.gui = false
  
    # Customize the amount of memory on the VM:
    vb.memory = "1024"
   end


end
