# PCI-DSS Compatible EFK stack
Done to provide log aggregation for several applications, their development environments, UAT, production environments


## Provides

* Ansible role to manage the system and kernel parameterns on each host
* Two Fluentd Aggregator Nodes done as Docker Containers
* Three ElasticSearch Master Node Cluster, done as Docker Containers
* Two ElasticSearch Data Node, done as Docker Containers
* ElasticSearch CrossCluster Search Node, done as Docker Container
* Kibana Node, done as Docker Container
* SearchGuard Implementation on ElasticSearch Nodes and Kibana node, done as Docker Container that can be deployed to an ElasticSearch node and used there to manage the SearchGuard implementation
* Apache Curator for managing the ES Data
* SearchGuard installation done with ActiveDirectory integration
* everything is secured with SSL certificates
* Docker Role
* Clean Role - for cleaning the damage done to all nodes : )


## Requires

1. Ansible
2. CentOS 6.5 later (or RedHat)
3. Docker latest

## Usage
Adapt hosts.yml and run `ansible-playbook -i hosts.yml efk.yml`
