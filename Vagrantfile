# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  config.vm.provision "ansible" do |ansible|
    ansible.groups = {
      'main' => ['default']
    }

    ansible.verbose = "v"
    ansible.playbook = ""
  end
end
