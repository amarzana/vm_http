Vagrant.configure("2") do |config|
	config.vm.define :http01 do |http01|
  		http01.vm.box = "ubuntu/yakkety64"
		http01.vm.hostname = "http01"
  		http01.vm.network "public_network", ip: "192.168.12.211"
		http01.vm.provision :shell, path: "bootstrap.sh"
	end
        config.vm.define :http02 do |http02|
                http02.vm.box = "ubuntu/yakkety64"
                http02.vm.hostname = "http02"
                http02.vm.network "public_network", ip: "192.168.12.212"
		http02.vm.provision :shell, path: "bootstrap.sh"
	end
end
