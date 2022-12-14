# network-engineer-19

Your company has several internal teams that create and manage their own projects and resources in Google Cloud. After a recent vulnerability report revealed suspicious network activity, your manager wants to secure and monitor the network usage of Google Cloud services. You want to follow Google-recommended practices to only allow external ingress VPC traffic based on specific API requests. What should you do?

A. Configure a new VPC firewall rule to deny service account access to the required Google services.

B. Create a hierarchical firewall for your existing organization, and add a new rule to allow egress traffic based on the IP address.

C. Use VPC Service Controls in enforced mode to create a service perimeter for your existing organization. Configure a new ingress policy to allow the required Google services. Review audit logs to verify traffic flow.

D. Use VPC Service Controls in dry run mode to create a service perimeter for your existing organization. Configure a new egress policy to allow access to the required Google Cloud services. Review audit logs to verify traffic flow.

## Feedback

A is not correct because configuring VPC firewall rules on a service account only allows or denies access on IPv4 or IPv6 connections, not on specific APIs for Google services.

B is not correct because the purpose of creating a hierarchical firewall is to allow or deny connections from IPv4 or IPv6 connections.

C is not correct because VPC Service Controls in enforced mode automatically enforces the policy without testing it first, and configuring an internal ingress policy won’t provide external API access.

D is correct because using VPC Service Controls to create a service perimeter lets you control access to Google services from inside and outside your VPC. It is recommended practice to test your policy in dry run mode before using enforced mode.

https://cloud.google.com/vpc-service-controls/docs/overview#isolate

https://cloud.google.com/vpc-service-controls/docs/create-service-perimeters

https://cloud.google.com/vpc-service-controls/docs/vpc-accessible-services

https://cloud.google.com/vpc-service-controls/docs/troubleshooting