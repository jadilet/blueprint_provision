# Wordpress blueprint provisioning
If you would need a running wordpress on your machine, you don't have to necessarily register a peer into bazaar. There is a way to bring it up directly in your machine. This wiki page will be guiding you through the process. 

Blueprint provisioning can be implemented via [Vagrant](https://www.vagrantup.com/) and [Vagrant Subutai plugin](https://github.com/subutai-io/vagrant).

First, you need to create a directory where you would like to bring your peer up. After the directory is available, we need to make sure that there are the following files:

# Vagrantfile
This file consists of the box parameters. The box's name is [subutai/stretch](https://app.vagrantup.com/subutai/boxes/stretch) (Debian based box).

# Subutai.json
This is blueprint file. You can use blueprint from [here](https://github.com/subutai-blueprints).

# vagrant-subutai.yml

This is user configuration parameter file. For more info you can visit this [page](https://github.com/subutai-io/vagrant/wiki/Configuration-Parameters). 

# Let's run blueprint provisioning:
(Here [wiki](https://github.com/subutai-io/vagrant/wiki/How-to-Install-and-Use-Vagrant-Providers) about. How to Install and Use Vagrant Providers.)

If you have the subutai peer then put `Subutai.json` and `vagrant-subutai.yml` files right to the next to `Vagrantfile` file
and execute following command:

`vagrant provision`

If you don't have peer, just execute following command:

`vagrant up`

So, now you should have a peer with blueprint available in it! 

