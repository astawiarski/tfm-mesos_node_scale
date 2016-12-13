# Input Variable

## Global

* cluster_name: Name of the cluster (must be uniq per region)

## AWS

* security_group: Security Group to access Mesos Cluster
* subnets: Subnets of The cluster
* mesos_node: Name of the ASG for node

## Lambda setup

* node_gather_handler: lambda handler for gather function
* node_process_handler: lambda handler for process function
* node_scale_handler: lambda handler for scale function

## Lambda configuration

* scale_down_threshold: Threashold in % to trigger a scale down
* scale_up_threshold: Threashold in % to trigger a scale up
* cpu_resource: Number of cpu per Node
* mem_resource: Number of mem per Node
* agent_min_capacity: Minimum number of agent that the cluster must not get 
lower
* rate_limit: max rate of scaling

## Mesos 

* mesos_master: Fqdn of the mesos-master endpoint
