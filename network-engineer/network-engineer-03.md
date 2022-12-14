# network-engineer-03

You work at an enterprise company that wants to enforce central management of all Google Cloud firewall rules. Currently, each internal business unit uses folders to manage their Google Cloud projects and network. You want the ability to deny incoming requests to the business unit's Compute Engine VMs. What should you do?

A. Configure VPC firewall rules to deny and allow traffic.

B. Create a Shared VPC network, and configure the firewall in the host project.

C. Create a hierarchical firewall policy at the organization level, and allow all egress traffic to the required business unit.

D. Create a hierarchical firewall policy at the organization level, and deny all ingress traffic to the required business unit.

## Feedback

A is not correct because creating a VPC will not let you enforce firewall policies across the organization.

B is not correct because creating a Shared VPC network will not let you enforce firewall policies across the organization.

C is not correct because creating a hierarchical firewall policy at the organization level and allowing egress traffic will not apply a policy to incoming requests.

D is correct because hierarchical firewall policies let you create and enforce a consistent firewall policy across your organization. You can assign hierarchical firewall policies to the entire organization, or to individual folders. These policies contain rules that can explicitly deny or allow ingress and egress connections.

https://cloud.google.com/vpc/docs/firewall-policies?hl=en

https://cloud.google.com/vpc/docs/firewall-policies-examples#example_4_configure_organization-wide_and_folder-specific_rules