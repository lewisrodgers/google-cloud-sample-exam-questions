# security-engineer-04

A customer needs to rely on their existing user directory with the requirements of native authentication when developing solutions in Google Cloud. They want to leverage their existing tooling and functionality to gather insight on user activity from a familiar interface. Which action should you take to meet the customer's requirements?

A. Provision users into Cloud Identity using Just-in-Time SAML 2.0 user provisioning with the customer User Directory as source.

B. Configure Cloud Identity as a SAML 2.0 Service Provider, using the customer's User Directory as the Identity Provider.

C. Configure and enforce 2-Step Verification in Cloud Identity for all Super Admins.

D. Configure a third-party IdP (Octa or Ping Federate) to manage authentication.

## Feedback

A is not correct because the client wants to continue using their existing directory.

B is correct because it lets the client use their current user directory as source of truth and to be authenticated against while using Cloud identity as their SAML broker.

C is not correct because it adds protection to super admin account but doesn’t address the use case.

D is not correct because it proposes a non-native solution and doesn’t address the use case.

https://cloud.google.com/blog/products/identity-security/using-your-existing-identity-management-system-with-google-cloud-platform

https://support.google.com/a/answer/60224