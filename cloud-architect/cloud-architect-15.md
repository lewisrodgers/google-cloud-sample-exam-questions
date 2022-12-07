# cloud-architect-15

Your organization has a 3-tier web application deployed in the same Google Cloud Virtual Private Cloud (VPC). Each tier (web, API, and database) scales independently of the others. Network traffic should flow through the web to the API tier, and then on to the database tier. Traffic should not flow between the web and the database tier. How should you configure the network with minimal steps?

A. Add each tier to a different subnetwork.

B. Set up software-based firewalls on individual VMs.

C. Add tags to each tier and set up routes to allow the desired traffic flow.

D. Add tags to each tier and set up firewall rules to allow the desired traffic flow.

## Feedback

A is not correct because the subnetwork alone will not allow and restrict traffic as required without firewall rules.

B is not correct because this adds complexity to the architecture and the instance configuration.

C is not correct because routes still require firewall rules to allow traffic as requests. Additionally, the tags are used for defining the instances the route applies to, and not for identifying the next hop. The next hop is either an IP range or instance name, but in the proposed solution the tiers are only identified by tags.

D is correct because as instances scale, they will all have the same tag to identify the tier. These tags can then be leveraged in firewall rules to allow and restrict traffic as required, because tags can be used for both the target and source.

https://cloud.google.com/vpc/docs/using-vpc

https://cloud.google.com/vpc/docs/routes

https://cloud.google.com/vpc/docs/add-remove-network-tags