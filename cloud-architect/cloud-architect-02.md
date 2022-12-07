# cloud-architect-02

For this question, refer to the [EHR Healthcare case study](https://services.google.com/fh/files/blogs/master_case_study_ehr_healthcare.pdf).

EHR wants to connect one of their data centers to Google Cloud. The data center is in a remote location over 100 kilometers from a Google-owned point of presence. They can't afford new hardware, but their existing firewall can accommodate future throughput growth. They also shared these data points:

- Servers in their on-premises data center need to talk to Google Kubernetes Engine (GKE) resources in the cloud.
- Both on-premises servers and cloud resources are configured with private RFC 1918 IP addresses.
- The service provider has informed the customer that basic Internet connectivity is a best-effort service with no SLA.

You need to recommend a connectivity option. What should you recommend?

A. Provision Carrier Peering.

B. Provision a new Internet connection.

C. Provision a Partner Interconnect connection.

D. Provision a Dedicated Interconnect connection.

## Feedback

A is not correct because it does not give private IP addressing across the connection.

B is not correct because an additional Internet connection will not provide RFC1918 communications by itself.

C is correct because it allows the customer to lower latency by connecting directly to a partner network that is directly connected to Google. This option will also allow the customer to use the lower bandwidth interfaces that they have on their current firewall.

D is not correct because Dedicated Interconnect would require the customer to buy new hardware to get a 10 gig interface for their firewall.

https://cloud.google.com/blog/products/networking/google-cloud-network-connectivity-options-explained

https://cloud.google.com/interconnect/docs/how-to/carrier-peering#considerations

https://cloud.google.com/interconnect/docs/concepts/partner-overview

https://cloud.google.com/interconnect/docs/concepts/dedicated-overview#before_you_use