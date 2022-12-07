# security-engineer-14

Your customer is moving their corporate applications to Google Cloud. The security team wants detailed visibility of all resources in the organization. You use Resource Manager to set yourself up as the org admin. What Cloud Identity and Access Management (Cloud IAM) roles should you give to the security team?

A. Org viewer, Project owner

B. Org viewer, Project viewer

C. Org admin, Project browser

D. Project owner, Network admin

## Feedback

A is not correct because Project owner is too broad. The security team does not need to be able to make changes to projects.

B is correct because:
- Org viewer grants the security team permissions to view the organization's display name.
- Project viewer grants the security team permissions to see the resources within projects.

C is not correct because Org admin is too broad. The security team does not need to be able to make changes to the organization.

D is not correct because Project owner is too broad. The security team does not need to be able to make changes to projects.

https://cloud.google.com/resource-manager/docs/access-control-org#using_predefined_roles