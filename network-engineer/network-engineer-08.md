# network-engineer-08

Your company is planning an upcoming migration from a large enterprise on-premises data center to Google Cloud. Because the current on-premises network is managed by the local network team, you want to design the cloud network for future growth while ensuring that several internal teams can start working quickly on Google Cloud. What should you do?

A. Create a Shared VPC network with a single host project.

B. Create a Shared VPC network with multiple host projects.

C. For each internal team, create a VPC network with a /8 CIDR block.

D. Create one project that has five VPC networks, each with a /28 CIDR block.

## Feedback

A is not correct because using a single host project would potentially limit your growth because you could reach your project quota too quickly .

B is correct because in cases where the aggregate resource requirements of all VPC networks can't be met within a project's quota, you should use an architecture with multiple host projects and set up a single Shared VPC network per host project.

C is not correct because this solution would require more effort to create the networks, which would not allow your internal teams to start operating quickly.

D is not correct because one project with a /28 CIDR block would not be suitable for future growth because it would provide only 16 total IP addresses.

https://cloud.google.com/architecture/best-practices-vpc-design#multiple-host-quota

https://cloud.google.com/vpc/docs/quota#shared-vpc