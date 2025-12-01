
Vagrant.configure("2") do |config|

  config.vm.box = "debian/bullseye64"
  config.vm.network "private_network", ip: "192.168.56.101"
  config.vm.provision "shell", path: "bootstrap.sh"
  config.vm.synced_folder "C:/Users/pacop/Documentos/DAW/2DAW/DAWEB/Nginx-II/html", "/var/www/paco.test/html"
end
