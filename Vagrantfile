# -*- mode: ruby -*-
# vi: set ft=ruby :

nodejs_install_method = ENV.key?('NODEJS_INSTALL_METHOD') ? ENV['NODEJS_INSTALL_METHOD'] : 'source'

Vagrant.configure('2') do |config|
  # Ensure we use our vagrant private key
  config.ssh.insert_key = false
  config.ssh.private_key_path = '~/.vagrant.d/insecure_private_key'

  config.vm.define 'anxs' do |machine|
    machine.vm.box = "hashicorp/trusty64"

    machine.vm.network :private_network, ip: '192.168.88.17'
    machine.vm.hostname = 'anxs.local'
    machine.vm.provision 'ansible' do |ansible|
      ansible.playbook = 'test.yml'
      ansible.become = true
      ansible.inventory_path = 'vagrant-inventory'
      ansible.host_key_checking = false
      ansible.extra_vars = {
        nodejs_install_method: nodejs_install_method
      }
    end
  end
end
