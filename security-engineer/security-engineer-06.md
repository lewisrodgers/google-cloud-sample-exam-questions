# security-engineer-06

Your team creates an ingress firewall rule to allow SSH access from their corporate IP range to a specific bastion host on Compute Engine. Your team wants to make sure that this firewall rule cannot be used by unauthorized engineers who may otherwise have access to manage VMs in the development environment. What should your team do to meet this requirement?

A. Create the firewall rule with a target of a network tag. Centrally manage access to the tag.

B. Create the firewall rule with a target of a service account. Centrally manage access to the service account.

C. Create the firewall rule in a Shared VPC with a target of a network tag.

D. Create the firewall rule in a Shared VPC with a target of a specific subnet.

## Feedback

A is not correct because the network tag value can be inferred by examining the Firewall Rule or VM metadata.

B is correct because access to the Service Account is required to use a firewall rule with a target of a Service Account.

C is not correct because the target network tag value can be inferred by examining the Firewall Rule or VM metadata.

D is not correct because the target subnet value can be inferred by examining the Firewall Rule or VM metadata.

https://cloud.google.com/vpc/docs/firewalls#service-accounts-vs-tags