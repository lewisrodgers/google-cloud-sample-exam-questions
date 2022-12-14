# network-engineer-04

Your customer has SaaS applications on Google Cloud. You want your services to be available to the customers' application in the most secure and cost-effective way. What should you do?

A. Configure a Cloud VPN gateway that provides a connection into their Google Cloud VPC network.

B. Create a Cloud Identity account to give you access into their Google Cloud VPC network.

C. Configure VPC Network Peering to connect directly into their Google Cloud VPC network.

D. Create a custom HTTP application that provides a connection to their Google Cloud VPC network.

## Feedback

A is not correct because using Cloud VPN incurs additional egress costs.

B is not correct because creating only a Cloud Identity account does not give you enough access to support your customer’s applications.

C is correct because VPC Network Peering enables you to connect VPC networks so that workloads in different VPC networks can communicate internally. Traffic stays within Google's network and doesn't traverse the public internet.

D is not correct because creating a custom HTTP application requires software development and is not cost-effective.


https://cloud.google.com/vpc/docs/vpc-peering