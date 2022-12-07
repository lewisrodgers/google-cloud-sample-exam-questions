# cloud-architect-13

Your company wants to try out the cloud with low risk. They want to archive approximately 100 TB of their log data to the cloud and test the serverless analytics features available to them there, while also retaining that data as a long-term disaster recovery backup. Which two steps should they take? (Choose two)

A. Load logs into BigQuery.

B. Load logs into Cloud SQL.

C. Import logs into Cloud Logging.

D. Insert logs into Cloud Bigtable.

E. Upload log files into Cloud Storage.

## Feedback

A is correct because BigQuery is a serverless cloud data warehouse for analytics and supports the volume and analytics requirement.

B is not correct because Cloud SQL does not support the expected 100 TB. Additionally, Cloud SQL is a relational database and not the best fit for time-series log data formats.

C is not correct because Cloud Logging is optimized for monitoring, error reporting, and debugging instead of analytics queries.

D is not correct because Cloud Bigtable is optimized for read-write latency and analytics throughput, not analytics querying and reporting.

E is correct because Cloud Storage provides the Coldline and Archive storage classes to support long-term storage with infrequent access, which would support the long-term disaster recovery backup requirement.

https://cloud.google.com/storage/docs/storage-classes

https://cloud.google.com/bigtable/

https://cloud.google.com/products/operations

https://cloud.google.com/sql/

https://cloud.google.com/bigquery/