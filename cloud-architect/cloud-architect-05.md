# cloud-architect-05

For this question, refer to the [Mountkirk Games case study](https://services.google.com/fh/files/blogs/master_case_study_mountkirk_games.pdf).

You are the data compliance officer for Mountkirk Games and must protect customers' personally identifiable information (PII). Mountkirk Games wants to make sure they can generate anonymized usage reports about their new game and delete PII data after a specific period of time. The solution should have minimal cost. You need to ensure compliance while meeting business and technical requirements. What should you do?

A. Archive audit logs in Cloud Storage, and manually generate reports.

B. Write a Cloud Logging filter to export specific date ranges to Pub/Sub.

C. Archive audit logs in BigQuery, and generate reports using Google Data Studio.

D. Archive user logs on a locally attached persistent disk, and cat them to a text file for auditing.

## Feedback

A is not correct because Cloud Storage is an object store with no query language access for report generation.

B is not correct because it does not address log storage for data retention.

C is correct because BigQuery allows easy querying for report generation, with low storage costs.

D is not correct because long term storage in persistent disks is expensive.

https://cloud.google.com/security/compliance/soc-2

https://cloud.google.com/logging/docs/audit

https://cloud.google.com/bigquery/docs/cached-results

https://cloud.google.com/logging/docs/view/available-logs