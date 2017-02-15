# ac-etcd

This is a prototype of etcd cluster deployed and managed by the AppController

Usage:

`kubeac run etcd-bootstrap --arg=initialClusterSize=3`

to deploy,

`kubeac run etcd-scale --factor=2`

to add 2 extra nodes,

`kubeac run etcd-scale --factor=2 --undo`

to remove 2 nodes,

`kubeac get replicas etcd-nodes`

to get list of cluster node IDs,

`kubeac run etcd-scale --undo --replica=$NODE_ID`

to delete some particular node,

`kubeac run etcd-bootstrap --undo`

to delete the entire cluster.
