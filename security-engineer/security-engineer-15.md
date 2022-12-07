# security-engineer-15

Your company wants to collect and analyze CVE information for packages in container images, and wants to prevent images with known security issues from running in your Google Kubernetes Engine environment. Which two security features does Google recommend including in a container build pipeline? (choose two)

A. Deployment policies

B. Password policies

C. Vulnerability scanning

D. Network isolation

## Feedback

A is correct because deployment policies defined in Binary Authorization ensure that only trusted images can be deployed in Google Kubernetes Engine clusters. Binary Authorization can integrate with Container Analysis which scans container images stored in Container Registry for vulnerabilities and stores trusted metadata used in the authorization process.

B is not correct because it doesn’t address the use case.

C is correct because vulnerability scanning can be performed by Container Analysis to discover package vulnerability information in container base images and obtain CVE data from respective Linux distributions.

D is not correct because it doesn’t address the use case.

https://cloud.google.com/binary-authorization/docs/overview

https://cloud.google.com/con