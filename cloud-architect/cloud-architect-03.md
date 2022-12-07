# cloud-architect-03

For this question, refer to the [EHR Healthcare case study](https://services.google.com/fh/files/blogs/master_case_study_ehr_healthcare.pdf).

One of EHR’s healthcare customers is an internationally renowned research and hospital facility. Many of their patients are well-known public personalities. Sources both inside and outside have tried many times to obtain health information on these patients for malicious purposes. The hospital requires that patient information stored in Cloud Storage buckets not leave the geographic areas in which the buckets are hosted. You need to ensure that information stored in Cloud Storage buckets in the "europe-west2" region does not leave that area. What should you do?

A. Encrypt the data in the application on-premises before the data is stored in the "europe-west2" region.

B. Enable Virtual Private Network Service Controls, and create a service perimeter around the Cloud Storage resources.

C. Assign the Identity and Access Management (IAM) "storage.objectViewer" role only to users and service accounts that need to use the data.

D. Create an access control list (ACL) that limits access to the bucket to authorized users only, and apply it to the buckets in the "europe-west2" region.

## Feedback

A is not correct because encrypting the data does not stop data exfiltration.

B is correct because VPC Service Controls improves your ability to mitigate the risk of data exfiltration from Google Cloud services.

C is not correct because IAM roles deal with identity-based access control, not context-aware perimeter security.

D is not correct because Cloud Storage ACLs are a mechanism you can use to define who has access to your buckets and objects, as well as their level of access. ACLs do not stop data exfiltration.

https://cloud.google.com/vpc-service-controls/docs/overview

https://cloud.google.com/storage/docs/access-control/lists