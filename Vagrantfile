Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.ssh.forward_x11 = true
  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

  # config.vm.network "private_network", ip: "192.168.33.10"

  # config.vm.network "public_network"

  # config.vm.synced_folder "../data", "/vagrant_data"

  config.vm.provider "virtualbox" do |new_vm|
  #   # Display the VirtualBox GUI when booting the machine
  #   new_vm.gui = true
    new_vm.name = "New_Vm"
  #   # Customize the amount of memory on the VM:
    new_vm.customize ["modifyvm", :id, "--memory", "2048", "--cpus", "2"]
  end

  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
