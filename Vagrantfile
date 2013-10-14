Vagrant::Config.run do |config|
  config.vm.box = 'raring64'
  config.vm.box_url = 'http://goo.gl/Y4aRr'
  config.vm.provision :puppet,
    :module_path => 'modules' do |puppet|
      puppet.manifest_file = 'manifest.pp'
  end
end
