# network-engineer-09

Your organization recently deployed several private Google Kubernetes Engine (GKE) clusters. You notice that the control planes of some of your GKE clusters can be accessed from any IP address. You want to restrict network access to the control plane while minimizing infrastructure changes. What should you do?

A. Create a new GKE cluster with authorized networks enabled.

B. Create a new GKE private cluster with authorized networks enabled.

C. Enable a new authorized network by updating your existing GKE private cluster.

D. Enable a new authorized network by updating the external IP address range of your existing cluster.

## Feedback

A is not correct because creating a new GKE cluster requires infrastructure changes.

B is not correct because creating a new GKE cluster requires infrastructure changes.

C is correct because authorized networks let you specify CIDR ranges and allow IP addresses in those ranges to access your cluster control plane endpoint by using HTTPS. An authorized network to an existing cluster can be added by using the gcloud CLI or the Google Cloud Console.

D is not correct because, although updating the external IP address range lets you grow or shrink the address range, it does not restrict network access.

https://cloud.google.com/kubernetes-engine/docs/how-to/authorized-networks#overview.

https://cloud.google.com/kubernetes-engine/docs/how-to/authorized-networks#add