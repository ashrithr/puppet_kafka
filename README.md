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

###Usage:

To Install and configure kafka:

```puppet
class { 'kafka':
    hosts => {
         'kafka-node01.domain.org' => { 'id' => 1 },
         'kafka-node02.domain.org' => { 'id' => 2 },
     },
     zookeeper_hosts => ['zk-node01:2181', 'zk-node02:2181','zk-node03:2181'],
 }
```

(Or) if the data is available from hiera: `include kafka`
