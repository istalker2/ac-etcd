# ac-etcd

This is a prototype of etcd cluster deployed and managed by the AppController

Use

kubeac run etcd-bootstrap --arg=initialClusterSize=3

to deploy and then

kubeac run etcd-scale --factor=2

to add 2 extra nodes
