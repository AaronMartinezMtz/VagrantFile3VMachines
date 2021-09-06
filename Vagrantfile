# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  
	
	config.vm.define :ldap do |ldap|
          ldap.vm.box       = "freebsd11"
          ldap.vm.box_url   = "https://app.vagrantup.com/generic/boxes/freebsd11/versions/3.4.2/providers/parallels.box"
          ldap.vm.host_name = "ldap.vm"
          ldap.vm.network :hostonly, "192.168.56.11"
          ldap.vm.provision :shell, :path => "puppet.sh"
	end
	
	
		config.vm.define :ldap1 do |ldap1|
          ldap1.vm.box       = "ubuntu1404-x64"
          ldap1.vm.box_url   = "https://app.vagrantup.com/puphpet/boxes/ubuntu1404-x64/versions/20161102/providers/parallels.box"
          ldap1.vm.host_name = "ldap1.vm"
          ldap1.vm.network :hostonly, "192.168.56.11"
          ldap1.vm.provision :shell, :path => "puppet.sh"
	end
	
	
		config.vm.define :ldap2 do |ldap2|
          ldap2.vm.box       = "centos7"
          ldap2.vm.box_url   = "https://app.vagrantup.com/generic/boxes/centos7/versions/3.4.2/providers/parallels.box"
          ldap2.vm.host_name = "ldap2.vm"
          ldap2.vm.network :hostonly, "192.168.56.11"
          ldap2.vm.provision :shell, :path => "puppet.sh"
	end
	
  

  
end
