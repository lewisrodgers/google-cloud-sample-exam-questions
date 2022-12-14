# network-engineer-17

After a recent Google Kubernetes Engine (GKE) upgrade, you notice that some of your applications are not receiving expected traffic from the ingress. What should you do to troubleshoot the applications?

A. Create a new VPC and enable VPC Flow Logs and Cloud Logging. Validate the traffic path to the backends.

B. Create a new test GKE cluster with Cloud Logging and Cloud Monitoring enabled. Generate test scenarios.

C. Create a log bucket. Check the HTTPS ingress resource logs in Cloud Logging to validate the traffic to the backends.

D. Modify your existing GKE cluster and enable Cloud Logging and Cloud Monitoring. Export logs to BigQuery for analysis.

## Feedback

A is not correct because creating a new VPC will not help you troubleshoot your existing ingress traffic problems. A new VPC is a new configuration unrelated to your existing deployment.

B is not correct because Cloud Logging and Cloud Monitoring are already enabled by default. Creating a new GKE cluster with test scenarios will not help isolate the traffic problem with the current ingress. A new GKE cluster is a new configuration unrelated to your existing deployment.

C is correct because creating a specific log bucket to capture the logs lets you keep and analyze the usage metrics, which will allow you to discover the problem.

D is not correct because Cloud Logging and Cloud Monitoring are already enabled by default.

https://cloud.google.com/stackdriver/docs/solutions/gke/managing-logs

https://cloud.google.com/logging/docs/buckets

https://cloud.google.com/kubernetes-engine/docs/how-to/ingress-features