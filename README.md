# Wordpress blueprint provisioning

Blueprint provisioning via [Vagrant](https://www.vagrantup.com/) and [Vagrant Subutai plugin](https://github.com/subutai-io/vagrant).

# Vagrantfile
Box name is [subutai/stretch](https://app.vagrantup.com/subutai/boxes/stretch) (Debian based box).

# Subutai.json
It is blueprint file. You can use blueprint from [here](https://github.com/subutai-blueprints).

# vagrant-subutai.yml

It is user configuration parameter file. More info you can visit [here](https://github.com/subutai-io/vagrant/wiki/Configuration-Parameters). 

# Let's run blueprint provisioning:
(Here [wiki](https://github.com/subutai-io/vagrant/wiki/How-to-Install-and-Use-Vagrant-Providers) about. How to Install and Use Vagrant Providers.)

If you have the subutai peer then put `Subutai.json` and `vagrant-subutai.yml` files to the next to `Vagrantfile` file
and execute following command:

`vagrant provision`

If you don't have peer, just execute following command:

`vagrant up`



