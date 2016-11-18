Vagrant.configure("2") do |config|
  config.vm.box = "puppetlabs/centos-7.0-64-puppet"
  config.vm.network "private_network", ip: "192.0.2.2"
#  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"
#  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.network :forwarded_port, guest: 80, host: 4567
end