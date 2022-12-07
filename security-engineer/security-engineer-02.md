# security-engineer-02

A customer wants to use Cloud Identity as their primary IdP. The customer wants to use other non-Google Cloud SaaS products for CRM, messaging, and customer ticketing management. The customer also wants to improve employee experience with Single Sign-On (SSO) capabilities to securely access Google Cloud and non-Google Cloud applications. Only authorized individuals should be able to access these third-party applications. What action should the customer take to meet these requirements?

A. Remove the employee from Cloud Identity, set the correct license for the individuals, and resync them to Cloud Identity for the changes to take effect.

B. Configure third-party applications to federate authentication and authorization to the Google Cloud IdP.

C. Remove the individuals from the third-party applications, add the license to Cloud Identity, and resync the individuals back to the third-party applications.

D. Copy user personas from Cloud Identity to all third-party applications for the domain.

## Feedback

A is not correct because Users should continue to be in Cloud Identity as central source of truth.

B is correct because cloud identity will serve as SAML auth for third party apps.

C is not correct because it doesn’t help to automate user provisioning.

D is not correct because it doesn’t help to automate user provisioning and deprovisioning on a continual basis.

https://cloud.google.com/identity/solutions/enable-sso