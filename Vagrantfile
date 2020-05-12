Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"
    config.vm.define 'ubuntu'
    config.vm.boot_timeout = 600
    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--audio", "none"]
        vb.gui = false
        vb.name = 'vagrant'
        vb.memory = 512
        vb.cpus = 1
    end
end
