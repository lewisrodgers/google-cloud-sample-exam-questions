# cloud-architect-06

For this question, refer to the [Mountkirk Games case study](https://services.google.com/fh/files/blogs/master_case_study_mountkirk_games.pdf).

Mountkirk Games wants you to make sure their new gaming platform is being operated according to Google best practices. You want to verify that Google-recommended security best practices are being met while also providing the operations teams with the metrics they need. What should you do? (Choose two)

A. Ensure that you aren’t running privileged containers.

B. Ensure that you are using obfuscated Tags on workloads.

C. Ensure that you are using the native logging mechanisms.

D. Ensure that workloads are not using securityContext to run as a group.

E. Ensure that each cluster is running GKE metering so each team can be charged for their usage.

## Feedback

A is correct because this is High Priority according to Google best practices.

B is not correct because tags should be readable and useful to the operations teams when they are working on the clusters.

C is correct because this is High Priority according to Google best practices.

D is not correct because this may be required for some workloads.

E is not correct because although from a business process this may be useful it won’t impact the operations or security of the cluster.

https://cloud.google.com/solutions/best-practices-for-operating-containers