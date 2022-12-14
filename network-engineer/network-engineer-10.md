# network-engineer-10

You have deployed an application that has static data on Cloud CDN. You need to enable distributed denial-of-service (DDoS) protection for your origin server. What should you do?

A. Configure a zonal network endpoint group. Create and apply a Google Cloud Armor security policy to the external origin.

B. Delete your existing HTTP load balancer. Create a new HTTP load balancer. Create and apply a Google Cloud Armor security policy to the external origin.

C. Create an internal HTTP load balancer with a backend service that has a zonal network endpoint group. Create and apply a Google Cloud Armor security policy to the external origin.

D. Configure your existing external HTTP load balancer with a backend service that has an internet network endpoint group. Create and apply a Google Cloud Armor security policy to the external origin.

## Feedback

A is not correct because you need a load balancer to forward traffic to a backend Cloud CDN bucket that hosts the static data.

B is not correct because deleting your existing HTTP load balancer and creating a new one from scratch has no technical benefit.

C is not correct because you need a Layer 7 HTTPS load balancer with a Cloud CDN backend service to enable DDoS protection.

D is correct because Cloud CDN deployments configured with a backend service can be protected with a Google Cloud Armor policy.

https://cloud.google.com/armor/docs/common-use-cases#cdn-ddos-defense