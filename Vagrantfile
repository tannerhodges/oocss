# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "stubbornella"
  config.vm.box_url = "https://dl.dropbox.com/u/558452/vagrant/package.box"
  config.vm.network :forwarded_port, guest: 80, host: 8080
  config.vm.provision :shell, :path => "tools/vagrant/vagrant_user.sh"
end

