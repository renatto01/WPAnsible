Vagrant.configure("2") do |config|
  


  config.vm.box = "centos/7"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
  config.vm.network "forwarded_port", guest: 80, host: 8080 
  config.vm.network "private_network", ip: "192.168.33.10"

end
