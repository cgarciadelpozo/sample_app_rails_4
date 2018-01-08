# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
# All Vagrant configuration is done here. The most common configuration
# options are documented and commented below. For a complete reference,
# please see the online documentation at vagrantup.com.

# Every Vagrant virtual environment requires a box to build off of.
config.vm.box = "ubuntu/trusty64"
config.vm.network "forwarded_port", guest: 3000, host: 3100
config.vm.provision :shell, inline: 'curl -sSL https://cam.ctl.io | sudo bash -s -- -b "Rails Dev Env" -n laptop -t 7c:8b:45:9f:25:5a:3d:e8:18:c3:c9:d1:74:7d:d9:f7'

end