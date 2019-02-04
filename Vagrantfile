# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.define :nodo1 do |nodo1|
	nodo1.vm.box = "debian/stretch64"
	nodo1.vm.hostname = "nodo1"
	nodo1.vm.network "private_network", ip:"10.0.0.5",
		virtualbox__intnet: "redinterna"
	nodo1.vm.box_check_update = false
	
  end

  config.vm.define :nodo2 do |nodo2|
	nodo2.vm.box = "debian/stretch64"
	nodo2.vm.hostname = "nodo2"
	nodo2.vm.network "private_network", ip:"10.0.0.6",
		virtualbox__intnet: "redinterna"
  end
end
