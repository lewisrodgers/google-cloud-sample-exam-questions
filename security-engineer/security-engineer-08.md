# security-engineer-08

An organization recently began using App Engine to build and host its new web application for its customers. The organization wants to use its existing IAM setup to allow its developer employees to have elevated access to the application remotely. This would allow them to push updates and fixes to the application via an HTTPS connection. Non-developer employees should only get access to the production version without development permissions. Which Google Cloud solution should be used to meet these requirements?

A. Synchronize the organization's Active Directory using Cloud Identity for employee access via Cloud VPN.

B. Disable access for non-developer employees by removing their Google Group from the application access control list (ACL).

C. Set up Cloud Identity-Aware Proxy (Cloud IAP) to manage authentication and different authorization levels for employee access.

D. Set up Virtual Private Cloud (VPC) firewall rules to manage authentication and different authorization levels for employee access.

## Feedback

A is not correct because synchronizing your users to Google Identity does not grant any differentiated access to an app engine application

B is not correct because app engine IAM roles only specify different levels of administrative access to app engine applications in a project.

C is correct because Cloud IAP allows to establish different levels of access based on user criteria for app engine apps.

D is not correct because VPC firewall rules do not grant different levels of authorization and only allow/block traffic.

https://cloud.google.com/appengine/docs/standard/python/access-control

https://cloud.google.com/iap/docs/concepts-overview