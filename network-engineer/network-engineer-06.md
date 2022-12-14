# network-engineer-06

Your company currently has a routes-based VPC-native cluster created in Google Kubernetes Engine (GKE). Next year, you plan to deploy significantly more applications on GKE, which will use all the available IP addresses. You want to follow Google-recommended practices for better scaling. What should you do?

A. Create a public GKE cluster in Autopilot mode.

B. Create a new GKE cluster with an authorized network.

C. Create a new VPC-native cluster, and use a Shared VPC network.

D. Create a new routes-based cluster, and use a Shared VPC network.

## Feedback

A is not correct because a VPC-native cluster in Autopilot has a pre-configured pod limit.

B is not correct because a GKE cluster with an authorized network is used to improve security, not to provide better scalability.

C is correct because using a VPC-native cluster with a Shared VPC network is a Google-recommended practice. VPC-native clusters scale more easily without consuming routes and are a secure, centralized method to manage VPC networks.

D is not correct because a new routes-based cluster will not support the scalability needed to solve the problem because it does not let you use ranges outside RFC 1918.

https://cloud.google.com/kubernetes-engine/docs/best-practices/networking#vpc-native-clusters

https://cloud.google.com/kubernetes-engine/docs/how-to/flexible-pod-cidr#cidr_settings_for_clusters