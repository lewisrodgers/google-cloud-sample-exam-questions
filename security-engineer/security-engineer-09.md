# security-engineer-09

You have defined subnets in a VPC within Google Cloud. You need multiple projects to create Compute Engine instances with IP addresses from these subnets. What should you do?

A. Configure Cloud VPN between the projects.

B. Set up VPC peering between all related projects.

C. Change the VPC subnets to enable private Google access.

D. Use Shared VPC to share the subnets with the other projects.

## Feedback

A is not correct as Cloud VPN between projects does not provide you the functionality to share a subnet to host resources on.

B is not correct because peering two VPCs does allow traffic between the two shared networks, but it’s only bi-directional. Peered VPC networks remain administratively separate.

C is not correct because private Google access allows you to access APIs from a private IP, but it does not have any impact on creating Compute instances on a specific subnet.

D is correct because s Shared VPC allows you to share a VPC into multiple projects, keep administrative oversight in the host project, while restricting the other projects to only create VMs on IPs in the shared VPC.

https://cloud.google.com/vpc/docs/shared-vpc

https://cloud.google.com/vpc/docs/vpc-peering