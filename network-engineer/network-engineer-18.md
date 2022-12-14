# network-engineer-18

You created a new VPC and configured a firewall to be used for an upcoming Compute Engine application. After you deployed the application, you noticed that your pre-existing Compute Engine instances cannot connect to resources in the new VPC. What could be causing this problem?

A. You did not enable the Policy Troubleshooter API.

B. You did not enable Shared VPC to allow connectivity.

C. You did not peer the VPC networks to allow connectivity.

D. The new VPC was not created in the same region as the existing VPC.

## Feedback

A is not correct because enabling the Policy Troubleshooter API lets you troubleshoot IAM policies but does not let you share VPCs across two different networks.

B is not correct because Shared VPC lets you share VPC networks with other Google Cloud projects but does not let you share VPCs across two different networks.

C is correct because VPC peering lets you share VPCs across two different networks.

D is not correct. If the VPCs are not peered, resources within separate VPCs cannot communicate with each other even if the resources are in the same region.

https://cloud.google.com/vpc/docs/vpc-peering