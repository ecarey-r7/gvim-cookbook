# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.berkshelf.enabled = true
  condif.omnibus.chef_version = :latest

  config.vm.box = 'precise64'
  config.vm.box_url = 'http://files.vagrantup.com/precise64.box'
  config.vm.hostname = 'gvim-ubuntu'
  config.vm.network :private_network, ip: '33.33.33.10'
  config.ssh.max_tries = 40
  config.ssh.timeout   = 120

  config.vm.provision :chef_solo do |chef|
    chef.run_list = %w[recipe[gvim-cookbook::default]]
  end
end
