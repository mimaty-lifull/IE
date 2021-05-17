Vagrant.configure("2") do |config|
  config.vm.box = "win10"
  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
    vb.memory = "4096"
    vb.customize [
      'modifyvm',
      :id,
      "--clipboard",
      "bidirectional",
    ]
  end

  config.vm.guest = "windows"
  config.vm.synced_folder ".", "/vagrant", mount_options:['dmode=777','fmode=777']
  config.vm.boot_timeout = 600

  config.ssh.username = "user"
  config.ssh.password = "pass"
  config.ssh.insert_key = false
  config.ssh.shell = 'sh -l'
end