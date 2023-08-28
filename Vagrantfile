ENV['VAGRANT_DEFAULT_PROVIDER'] = "qemu"

# set synced directory
SYNCED_DIR = "src"

Vagrant.configure("2") do |config|
  config.vm.box = "perk/ubuntu-2204-arm64"

  # create directory if not exist
  if !Dir.exist?(SYNCED_DIR)
    Dir.mkdir(SYNCED_DIR)
  end

  # https://github.com/hashicorp/vagrant/issues/9567 
  config.vm.synced_folder SYNCED_DIR, "/#{SYNCED_DIR}", smb_username: "chaehan-um"

  config.vm.provision :shell, path: "bootstrap.sh"
end