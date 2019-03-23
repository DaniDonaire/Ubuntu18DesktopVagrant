Vagrant.configure("2") do |config|
  config.vm.box = "danidonaire/ubuntu18desktop"
  config.vm.box_version = "1"
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--cpuexecutioncap", "50"]
  end
end