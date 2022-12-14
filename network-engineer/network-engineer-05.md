# network-engineer-05

You need to create a Google Kubernetes Engine (GKE) cluster that prevents inbound external access. You want the cluster to allow certain nodes to have outbound internet access. What should you do?

A. Create a VPC-native cluster, and enable private nodes.

B. Create a private GKE cluster, and enable private nodes.

C. Create a private GKE cluster, and use Cloud NAT for external access.

D. Create a GKE cluster within a Shared VPC network, and create a firewall rule that allows external access for the node.

## Feedback

A is not correct because creating a VPC-native cluster will not allow external outbound access.

B is not correct because a private GKE cluster doesn’t have external outbound access by default.

C is correct because creating a private cluster that uses Cloud NAT is a best practice to prevent external access.

D is not correct because a Shared VPC network could allow external IP addresses to access the cluster.

https://cloud.google.com/kubernetes-engine/docs/how-to/private-clusters#other_configurations