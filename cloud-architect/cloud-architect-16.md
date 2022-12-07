# cloud-architect-16

You are designing a large distributed application with 30 microservices. Each of your distributed microservices needs to connect to a database backend. You want to store the credentials securely. Where should you store the credentials?

A. In the source code

B. In an environment variable

C. In a secret management system

D. In a config file that has restricted access through ACLs

## Feedback

A is not correct because storing credentials in source code and source control is discoverable, in plain text, by anyone with access to the source code. This also introduces the requirement to update code and do a deployment each time the credentials are rotated.

B is not correct because consistently populating environment variables would require the credentials to be available, in plain text, when the session is started.

C is correct because a secret management system such as Secret Manager is a secure and convenient storage system for API keys, passwords, certificates, and other sensitive data. Secret Manager provides a central place and single source of truth to manage, access, and audit secrets across Google Cloud.

D is not correct because instead of managing access to the config file and updating manually as keys are rotated, it would be better to leverage a key management system. Additionally, there is increased risk if the config file contains the credentials in plain text.

https://cloud.google.com/kubernetes-engine/docs/concepts/secret

https://cloud.google.com/secret-manager