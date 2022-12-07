# security-engineer-07

You want to protect the default VPC network from all inbound and outbound internet traffic. What action should you take?

A. Create a Deny All inbound internet firewall rule.

B. Create a Deny All outbound internet firewall rule.

C. Create a new subnet in the VPC network with private Google access enabled.

D. Create instances without external IP addresses only.

## Feedback

A is not correct because a Deny All inbound firewall is already part of the standard configuration and does not need to be added.

B is correct because all inbound traffic is already blocked, but all egress traffic is allowed by default. To prevent any outbound traffic an extra rule needs to be added.

C is not correct because private Google allows calls to Google managed APIs from private IP addresses, but it does neither prevent you from providing external IPs or any other outgoing traffic from your instances.

D is not correct because outbound traffic can still be coming from instances with private IPs if Cloud NAT is used.

https://cloud.google.com/nat/docs/overview

https://cloud.google.com/vpc/docs/private-access-options

https://cloud.google.com/vpc/docs/using-firewalls