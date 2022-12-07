# cloud-architect-04

For this question, refer to the [EHR Healthcare case study](https://services.google.com/fh/files/blogs/master_case_study_ehr_healthcare.pdf).

The EHR sales employees are a remote-based workforce that travels to different locations to do their jobs. Regardless of their location, the sales employees need to access web-based sales tools located in the EHR data center. EHR is retiring their current Virtual Private Network (VPN) infrastructure, and you need to move the web-based sales tools to a BeyondCorp access model. Each sales employee has a Google Workspace account and uses that account for single sign-on (SSO). What should you do?

A. Create an Identity-Aware Proxy (IAP) connector that points to the sales tool application.

B. Create a Google group for the sales tool application, and upgrade that group to a security group.

C. Deploy an external HTTP(S) load balancer and create a custom Cloud Armor policy for the sales tool application.

D. For every sales employee who needs access to the sales tool application, give their Google Workspace user account the predefined AppEngine Viewer role.

## Feedback

A is correct because Identity-Aware Proxy (IAP) connector allows you to manage access to HTTP-based apps outside of Google Cloud.

B is not correct because Google groups by themselves do not grant access to an application nor do they move an application to a beyond corp model.

C is not correct because Cloud Armor does not authenticate or authorize application access.

D is not correct because the application is installed in the datacenter, not in the AppEngine environment.

https://cloud.google.com/iap/docs/cloud-iap-for-on-prem-apps-overview