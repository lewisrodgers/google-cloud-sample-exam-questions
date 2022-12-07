# security-engineer-03

A Cloud Development team needs to use service accounts extensively in their local development. You need to provide the team with the keys for these service accounts. You want to follow Google-recommended practices. What should you do?

A. Implement a daily key rotation process that generates a new key and commits it to the source code repository every day.

B. Implement a daily key rotation process, and provide developers with a Cloud Storage bucket from which they can download the new key every day.

C. Create a Google Group with all developers. Assign the group the IAM role of Service Account User, and have developers generate and download their own keys.

D. Create a Google Group with all developers. Assign the group the IAM role of Service Account Admin, and have developers generate and download their own keys.

## Feedback

A is not correct because the source code repository isn’t the place to store keys that expire/change.

B is correct because it allows for centralized admin managed key rotation process and doesn’t delegate key creation to developers which is an easy and secure way to manage keys.

C is not correct because the Service Account User IAM role doesn’t allow for creation of keys.

D is not correct because this veers away from best practices as the keys would reside in a decentralized place and can be potentially leaked.

https://cloud.google.com/blog/products/gcp/help-keep-your-google-cloud-service-account-keys-safe

https://cloud.google.com/iam/docs/understanding-service-accounts#best_practices

https://cloud.google.com/iam/docs/creating-managing-service-account-keys