Vagrant.configure("2") do |config|
  #Set name of the box
  config.vm.box = "trusty64"
  #Give further customisation
  config.vm.provision :shell, :path => "vm_provision/provision-ubuntu-14.04.sh"
  #Set the network
  config.vm.network "private_network", ip: "192.168.33.10"
  #Set the CPU and Memory usage
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--cpuexecutioncap", "50", "--cpus", "1"]
    vb.memory = 2048
  end
end
