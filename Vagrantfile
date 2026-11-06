Vagrant.configure("2") do |config|

  config.vm.define "monitor01" do |monitor|

    monitor.vm.box = "ubuntu/jammy64"
    monitor.vm.hostname = "monitor01"

    monitor.vm.network "private_network",
      ip: "192.168.56.17"

    monitor.vm.provider "virtualbox" do |vb|
      vb.name = "Nagios-Zabbix-Monitor01"
      vb.memory = 2048
      vb.cpus = 2
    end

  end

end
