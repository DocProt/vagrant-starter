Vagrant.configure("2") do |config|
  config.vm.box = "vagrant/box"
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.hostname = "vagrantbox"
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--cpuexecutioncap", "50", "--cpus", "1"]
    vb.memory = 2048
  end
end
