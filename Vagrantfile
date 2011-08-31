Vagrant::Config.run do |config|
  
  # Configure a db server
  config.vm.define :db do |vm_config|

    vm_config.vm.host_name = "db.local"
    vm_config.vm.network("192.168.10.10")
    vm_config.vm.box = "lucid64"
    vm_config.vm.box_url = "http://files.vagrantup.com/lucid64.box"
    vm_config.vm.customize do |vm|
      vm.cpu_execution_cap = 80
    end
  end
end
