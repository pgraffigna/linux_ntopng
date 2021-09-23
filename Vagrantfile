Vagrant.configure("2") do |config|
  config.ssh.insert_key = false
  config.vm.synced_folder ".", "/vagrant", disabled: true
 
  config.vm.define "testing" do |t|
    t.vm.box = "geerlingguy/ubuntu2004"
    t.vm.hostname = "testing"
    t.vm.network "public_network"
  end

  config.vm.provider "virtualbox" do |vb|
    vb.name = "testing"
    vb.memory = "2048"
    vb.cpus = "1"
  end  
end


