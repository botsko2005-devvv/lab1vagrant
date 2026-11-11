
Vagrant.configure("2") do |config|

  # Перша ВМ: Ubuntu 20.04 (Web-сервер)
  config.vm.define "web" do |web|
    web.vm.box = "generic/ubuntu2004"
    web.vm.hostname = "web-server"

    web.vm.provider "vmware_desktop" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

  # Друга ВМ: Debian 11 (Сервер бази даних)
  config.vm.define "db" do |db|
    db.vm.box = "generic/debian11"
    db.vm.hostname = "db-server"

    db.vm.provider "vmware_desktop" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

end
