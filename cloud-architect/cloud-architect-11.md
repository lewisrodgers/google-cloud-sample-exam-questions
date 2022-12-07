# cloud-architect-11

You are designing a future-proof hybrid environment that will require network connectivity between Google Cloud and your on-premises environment. You want to ensure that the Google Cloud environment you are designing is compatible with your on-premises networking environment. What should you do?

A. Use the default VPC in your Google Cloud project. Use a Cloud VPN connection between your on-premises environment and Google Cloud.

B. Create a custom VPC in Google Cloud in auto mode. Use a Cloud VPN connection between your on-premises environment and Google Cloud.

C. Create a network plan for your VPC in Google Cloud that uses CIDR ranges that overlap with your on-premises environment. Use a Cloud Interconnect connection between your on-premises environment and Google Cloud.

D. Create a network plan for your VPC in Google Cloud that uses non-overlapping CIDR ranges with your on-premises environment. Use a Cloud Interconnect connection between your on-premises environment and Google Cloud.

## Feedback

A is not correct because the default VPC is a VPC with Auto Mode IP ranges, which has the same problem as answer C.

B is not correct because with Auto Mode IP Ranges there is no guarantee that the IP ranges will not overlap with your on premises environment, either now or in the future.

C is not correct because to ensure correct routing, ranges cannot overlap between environments.

D is correct because this ensures your on premises network is compatible with your Google Cloud VPC.

https://cloud.google.com/vpc/docs/vpc#ip-ranges