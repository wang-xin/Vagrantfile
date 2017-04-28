Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "public_network", ip: "192.168.50.150"
  config.vm.hostname = "vagrant-ubuntu-trusty-64"
  config.vm.synced_folder "./", "/app"
  config.vm.provider "virtualbox" do |vb|
    vb.cpus = "1"
    vb.memory = "1024"
    vb.name = "vagrant-ubuntu-trusty-64"
  end


  config.vm.provision "shell", inline: <<-SHELL
    apt-get update
  SHELL
end