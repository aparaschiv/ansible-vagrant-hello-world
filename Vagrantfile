# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "chriswayg/alpine-3.7-x86_64"

  config.vm.network "forwarded_port", guest: 8000, host: 8000
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
  end

end
