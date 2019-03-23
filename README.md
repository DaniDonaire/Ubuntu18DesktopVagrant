# Ubuntu18DesktopVagrant
Get a Ubuntu 18 Desktop from Vagrant box

You only need open a PowerShell or any terminal where vagrant works

- Run $vagrant init

- Edit the file and leave it with the following configuration:

```HTML

Vagrant.configure("2") do |config|
  config.vm.box = "danidonaire/ubuntu18desktop"
  config.vm.box_version = "1"
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--cpuexecutioncap", "50"]
  end
end

```
