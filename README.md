###Description

Installs kafka 0.8

This is a fork from wikimedia puppet-kafka module but with following
differences:
* Does not depends on packages
* Comes pre-built with compiled source (.tgz)
* Integrates with hiera

###Requirements:

* [Java module](https://github.com/ashrithr/puppet_java.git)
* [Zookeeper module](https://github.com/ashrithr/puppet_zookeeper.git)
