# network-engineer-12

Your organization has moved several workloads to Google Cloud. Your current DNS server is on-premises, and you determine how DNS resolution is performed. You want to follow Google-recommended practices and make DNS changes to support the hybrid environment without affecting the latency. What should you do?

A. Keep the DNS server on-premises.

B. Move all DNS resolution to Cloud DNS.

C. Use two DNS systems in a hybrid approach.

D. Move all DNS resolution to an external provider.

## Feedback

A is not correct. Keeping the DNS server on-premises may have performance implications because DNS requests from Google Cloud have higher latency.

B is not correct because it’s not a Google-recommended practice for a hybrid environment, and your current on-premises workloads would encounter higher latency when accessing Cloud DNS.

C is correct because the Google-recommended practice is to use a hybrid approach with two authoritative DNS systems. Authoritative DNS resolution for your private Google Cloud environment is done by Cloud DNS. Authoritative DNS resolution for on-premises resources is hosted by existing DNS servers on-premises.

D is not correct because it’s not a Google-recommended practice, and moving all DNS resolution to an external provider could cause higher latency.

https://cloud.google.com/dns/docs/best-practices#choose_where_dns_resolution_is_performed