Vagrant::Config.run do |config|
  config.vm.box = 'ubuntu_12.04_min'
  config.vm.box_url = 'http://puppet-vagrant-boxes.puppetlabs.com/ubuntu-server-12042-x64-vbox4210.box'
  config.vm.provision :puppet do |puppet|
    puppet.manifests_path = "manifests"
    puppet.manifest_file = "default.pp"
  end 
  config.vm.provision :puppet, :module_path => "modules"
end

Vagrant.configure("2") do |config|
  config.vm.synced_folder "~/Code", "/code"
end

