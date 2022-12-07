# cloud-architect-10

For this question, refer to the [TerramEarth case study](https://services.google.com/fh/files/blogs/master_case_study_terramearth.pdf).

You are the data compliance officer for TerramEarth and must protect customers' personally identifiable information (PII), like credit card information. TerramEarth wants to personalize product recommendations for its large industrial customers. You need to respect data privacy and deliver a solution. What should you do?

A. Use AutoML to provide data to the recommendation service.

B. Process PII data on-premises to keep the private information more secure.

C. Use the Cloud Data Loss Prevention (DLP) API to provide data to the recommendation service.

D. Manually build, train, and test machine learning models to provide product recommendations anonymously.

## Feedback

A is not correct because AutoML does not inherently provide data de-identification.

B is not correct because TerramEarth's requirements are to go into the cloud, not stay on-premises.

C is correct because Cloud DLP was specifically designed for this use case.

D is not correct because developing machine learning models is an excessive way to de-identify data.

https://cloud.google.com/dlp/docs/deidentify-sensitive-data

https://cloud.google.com/automl