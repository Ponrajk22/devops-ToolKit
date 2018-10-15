Vagrant.configure(2) do |config|
	config.vm.define "devops-ToolKit" do |devbox|
		devbox.vm.box = "ubuntu/xenial64"
    		devbox.vm.network "private_network", ip: "10.10.10.10"
    		#devbox.vm.hostname = "devops-ToolKit"
      		devbox.vm.provision "shell", path: "scripts/install_v1.sh"
    		devbox.vm.provider "virtualbox" do |v|
    		  v.memory = 2048 
    		  v.cpus = 2
    		end
	end
    config.vm.synced_folder "/Users/ponraj.krishnapandi/Documents/shared", "/mnt/macMount"
end
#echo "source scripts/bashrc" >> /home/vagrant/.bashrc/
