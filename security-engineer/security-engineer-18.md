# security-engineer-18

A cloud customer has an on-premises key management system and wants to generate, protect, rotate, and audit encryption keys with it. How can the customer use Cloud Storage with their own encryption keys?

A. Declare usage of default encryption at rest in the audit report on compliance

B. Upload encryption keys to the same Cloud Storage bucket

C. Use Customer Managed Encryption Keys (CMEK)

D. Use Customer-Supplied Encryption Keys (CSEK)

## Feedback

A is not correct because default encryption at rest uses Google-generated and Google-managed keys, hence does not address the use case.

B is not correct because you’ll first need the encryption keys in order to decrypt the data in this Cloud Storage Bucket, but you won’t be able to have these encryption keys until you actually decrypt it. Customer-supplied encryption keys are not stored on Google’s infrastructure.

C is not correct because it doesn’t address this scenario in which customer wants to use their own encryption keys from their own key management system. This option will however be valid if the customer wants to use Google-generated and customer-managed keys.

D is correct because you can choose to provide your own AES-256 key when using Cloud Storage. This key is known as a customer-supplied encryption key (CSEK). If you provide a CSEK, Cloud Storage does not permanently store your key on Google's servers or otherwise manage your key. Instead, you provide your key for each Cloud Storage operation, and your key is purged from Google's servers after the operation is complete. Cloud Storage stores only a cryptographic hash of the key so that future requests can be validated against the hash.

https://cloud.google.com/security/encryption-at-rest/

https://cloud.google.com/storage/docs/encryption/using-customer-supplied-keys

https://cloud.google.com/storage/docs/encryption/customer-supplied-keys

https://cloud.google.com/storage/docs/encryption/customer-managed-keys