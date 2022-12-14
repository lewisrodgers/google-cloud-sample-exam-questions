# network-engineer-20

Your financial organization needs to migrate 5 PB of data to Google Cloud while also maintaining the same level of network performance as your on-premises network. You need to set up a cost-effective Cloud Interconnect connection that will provide sufficient capacity and failover protection. What should you do?

A. Provision dual 10-gbps VLAN attachments in us-central1.

B. Provision a single 50-gbps VLAN attachment in us-central1.

C. Provision dual 50-gbps VLAN attachments in two different edge availability domains.

D. Provision dual 10-gbps VLAN attachments in two different edge availability domains.

## Feedback

A is not correct because you need two different edge availability domains for failover protection.

B is not correct because a single 50-gbps VLAN attachment will not provide sufficient capacity or failover protection. You need two different edge availability domains.

C is not correct because using 50-gbps VLAN attachments isn’t the most cost-effective option.

D is correct because Google-recommended practice is to provision your Cloud Interconnect connection and VLAN attachment capacity so that each edge availability domain has enough capacity for all your production workload.

https://cloud.google.com/network-connectivity/docs/interconnect/concepts/best-practices#scenario_1_sufficient_capacity