# security-engineer-17

An organization is working on their GDPR compliance strategy. It wants to ensure that controls are in place to ensure that personally identifiable information (PII) is stored in Cloud Storage buckets without third-party exposure.  Which Google Cloud solution should the organization use to verify that PII is stored in the correct place without exposing PII internally?

A. Cloud Storage Bucket Lock

B. Cloud Data Loss Prevention API

C. VPC Service Controls

D. Web Security Scanner

## Feedback

A is not correct because Bucket Lock feature is for protecting the data retention policy and doesn’t address the use case.

B is correct because Cloud Data Loss Prevention API can be used to inspect Cloud Storage buckets for PII.

C is not correct because while VPC Service Controls can allow customers to define security perimeters around Cloud Storage Buckets in order to mitigate data exfiltration risks, it’s not a tool to locate PIIs hence doesn’t address this use case.

D is not correct because Web Security Scanner is for App Engine, Compute Engine, and Google Kubernetes Engine applications and doesn’t address the use case.

https://cloud.google.com/storage/docs/bucket-lock

https://cloud.google.com/dlp/docs/inspecting-storage#inspecting-gcs

https://cloud.google.com/vpc-service-controls/

https://cloud.google.com/security-scanner/