# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  config.vm.define "gitlab01" do |i|
    i.vm.hostname = "gitlab01"  
    i.vm.network "private_network", ip: "192.168.11.11"

    i.vm.provider "virtualbox" do |vb|
      vb.memory = "8192"
    end

    i.vm.provision "ansible_local" do |ansible|
      ansible.playbook = "playbook/gitlab01.yml"
      ansible.inventory_path = "playbook/hosts/local"
      ansible.limit = "localnode"
    end
  end
end
