# network-engineer-07

Your company works with an external vendor who uses Google Cloud. You need to provide the vendor with access to your private Cloud SQL instance. You want to provide high-performance access while minimizing costs. What should you do?

A. Create and configure a Shared VPC network for your Google project.

B. Create a user account in Cloud Identity, and enforce 2-Step Verification.

C. Create and configure a VPC Network Peering connection with the vendor’s Google project.

D. Add the vendor's Google Account to an existing Cloud Identity group that has access to the Cloud SQL instance.

## Feedback

A is not correct because a Shared VPC connection won’t provide access to your organization.

B is not correct because Cloud Identity and 2-Step Verification will not provide high-performance access.

C is correct because using VPC Network Peering prevents additional charges and performs well.

D is not correct because a Cloud Identity group will not provide high-performance access.

https://cloud.google.com/architecture/best-practices-vpc-design#vpc-peering-limits