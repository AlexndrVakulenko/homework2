ENV['VAGRANT_SERVER_URL'] = 'https://vagrant.elab.pro'
Vagrant.configure("2") do |config|
  

	config.vm.box = "generic/rhel8"
	config.vm.hostname = "RHEL8"
	config.vm.network "public_network", type: "dhcp"
    config.vm.define "RHEL8"

  	config.vm.synced_folder ".","/vagrant", type: "virtualbox"

    config.vm.provider "virtualbox" do |vb|
    vb.gui = true
	vb.cpus=2   
    vb.memory = "1024"
   end
 
end
