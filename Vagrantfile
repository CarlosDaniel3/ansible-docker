Vagrant.configure("2") do |config|
  config.vm.define "ubuntu" do |ubuntu|
    ubuntu.vm.box = "ubuntu/focal64"
    ubuntu.vm.network "public_network", bridge: "wlp2s0", ip: "192.168.100.118"
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "main.yml"    
  end
end