# config

Postgresql
---
version 9.5

Add repo config
```
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'
```
Add GPG key
```
wget -q https://www.postgresql.org/media/keys/ACCC4CF8.asc -O - | sudo apt-key add -
```

Install
```
sudo apt-get update 
sudo apt-get install postgresql-9.5
```

MySQL
---
```
sudo apt-get install mysql-server 
```


Zookeeper
---

`sudo apt-get install zookeeper`
Config file at: `/etc/zookeeper/conf/zoo.cfg`

Or use Zookeeper in Kafka source 


Kafka
---
Follow this: http://www.bogotobogo.com/Hadoop/BigData_hadoop_Zookeeper_Kafka_single_node_Multiple_broker_cluster.php


Golang
---

Follow this: https://golang.org/doc/install
Don't forget to set `$GOROOT` and `$GOPATH` in `~/.profile` or `~/.bashrc` or `~/.zshrc` or Environment variables (Windows)
Ex:

```
export PROGRAM=/home/stackops/program
export GOROOT=$PROGRAM/go
export GOPATH=/home/stackops/go
export PATH=$PATH:$GOPATH/bin
export PATH=$PATH:$GOROOT/bin
```
