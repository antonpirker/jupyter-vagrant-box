# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Config
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "data-science-box"

  # Port forwarding
  config.vm.network "forwarded_port", guest: 8888, host: 8888

  # Provisioning
  config.vm.provision :shell, path: "scripts/provision-vagrant.sh"
  config.vm.provision :shell, path: "scripts/provision-vagrant-user.sh", privileged: false

  # Welcome message
  config.vm.post_up_message = "*****************************************\n\n" \
                              "    Welcome to your data science box!\n\n"  \
                              "    To access your Jupyter Notebook\n" \
                              "    point your browser to:\n\n" \
                              "        http://localhost:8888\n\n" \
                              "    Have fun!\n\n" \
                              "*****************************************"
end
