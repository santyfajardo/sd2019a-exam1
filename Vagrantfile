# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.ssh.insert_key = false
  config.vm.define :lb_server do |lb|
    lb.vm.box = "centos_7"
    lb.vm.network :private_network, ip: "192.168.56.101"
    lb.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "1", "--name", "lb_server" ]
    end
    config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "playbook.yml"
        "web_servers" => [
          {"ip":"192.168.56.102:8080"},
          {"ip":"192.168.56.103:8080"}
         ]
      }
    end
  end
  config.vm.define :wb_server_1 do |wb1|
    wb1.vm.box = "centos_7"
    wb1.vm.network :private_network, ip: "192.168.56.102"
    wb1.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "1", "--name", "wb_server_1_a" ]
    end
    config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "playbook.yml"
      
end
  end
  config.vm.define :wb_server_2 do |wb2|
    wb2.vm.box = "centos_7"
    wb2.vm.network :private_network, ip: "192.168.56.103"
    wb2.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "1", "--name", "wb_server_1_b" ]
    end
    config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "playbook.yml"
    end
  end
end
