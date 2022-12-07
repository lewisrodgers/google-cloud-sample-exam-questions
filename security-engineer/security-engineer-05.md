# security-engineer-05

A customer wants to grant access to their application running on Compute Engine to write only to a specific Cloud Storage bucket. How should you grant access?

A. Create a service account for the application, and grant the Storage Object Creator role at the project level.

B. Create a service account for the application, and grant the Storage Object Creator role at the bucket level.

C. Create a user account, authenticate with the application, and grant the Storage Object Admin role at the bucket level.

D. Create a user account, authenticate with the application, and grant the Storage Object Admin role at the project level.

## Feedback

A is not correct because doesn’t restrict scope to specific bucket

B is correct because provides the right permission and keeps the scope limited to bucket in question

C is not correct because using a user account goes against the recommended practice as it should be a machine/service account that should be handling the writing to bucket

D is not correct because using a user account goes against the recommended practice as it should be a machine/service account that should be handling the writing to bucket and it also widens the scope to storage wide which violates minimum required privilege rules

https://cloud.google.com/iam/docs/understanding-service-accounts#using_service_accounts_with_compute_engine