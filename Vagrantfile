Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.provision "docker" do |d|
  	d.build_image "/vagrant", args: "-t aloerina/hello"
  	d.run "aloerina/hello", args: "-d -t -v /vagrant:/temp/shared"
  end
end
