Vagrant.configure('2') do |config|
  config.ssh.private_key_path = '~/.ssh/id_rsa'
  config.vm.box = 'digital_ocean'
  config.vm.provider :digital_ocean do |provider|
    provider.image = 'Ubuntu 12.04 x32'
    provider.region = 'New York 1'
    provider.size = '512MB'
    provider.client_id = ENV['DO_CLIENT_ID']
    provider.api_key = ENV['DO_API_KEY']
  end

  config.omnibus.chef_version = :latest
 
end
