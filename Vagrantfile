# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "bento/centos-7.1"

  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.hostname = "node1"

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "playbook.yml"
  end


 #  #Install Zookeeper and the Zookeeper server package by pointing to the RPM repository for ZooKeeper:
 #  config.vm.provision "shell", inline: "sudo rpm -Uvh http://archive.cloudera.com/cdh4/one-click-install/redhat/6/x86_64/cloudera-cdh-4-0.x86_64.rpm"
 #  config.vm.provision "shell", inline: "sudo yum -y install zookeeper zookeeper-server"
 #  #Initialize and start Zookeeper:
 #  config.vm.provision "shell", inline: "sudo -u zookeeper zookeeper-server-initialize --myid=1"
 #  config.vm.provision "shell", inline: "sudo service zookeeper-server start"
end
