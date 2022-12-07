# security-engineer-12

Your company is storing files on Cloud Storage. To comply with local regulations, you want to ensure that uploaded files cannot be deleted within the first 5 years. It should not be possible to lower the retention period after it has been set. What should you do?

A. Apply a retention period of 5 years to the bucket, and lock the bucket.

B. Enable Temporary hold and apply a retention period of 5 years to the bucket.

C. Use Cloud IAM to ensure that nobody has an IAM role that has the permissions to delete files from Cloud Storage.

D. Create an object lifecycle rule using the Age condition and the Delete action. Set the Age condition to 5 years.

## Feedback

A is correct because Bucket Lock allows you to configure a data retention policy for a Cloud Storage bucket that governs how long objects in the bucket must be retained. The feature also allows you to lock the data retention policy, permanently preventing the policy from being reduced or removed.

B is not correct because object holds can be easily released by operators/admins.

C is not correct because an admin can grant themselves or someone else enough rights to tamper with the files in Cloud Storage.

D is not correct because Age condition and a Delete action does not prevent objects from being manually deleted before the Age condition is met.

https://cloud.google.com/storage/docs/bucket-lock