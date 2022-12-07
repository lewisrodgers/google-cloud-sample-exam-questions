# cloud-architect-01

For this question, refer to the [EHR Healthcare case study](https://services.google.com/fh/files/blogs/master_case_study_ehr_healthcare.pdf).

Anonymous users from all over the world access a public health information website hosted in an on-premises EHR data center. The servers that host this website are older, and users are complaining about sluggish response times. There has also been a recent increase of distributed denial-of-service attacks toward the website. The attacks always come from the same IP address ranges. EHR management has identified the public health information website as an easy, low risk application to migrate to Google Cloud. You need to improve access latency and provide a security solution that will prevent the denial-of-service traffic from entering your Virtual Private Cloud (VPC) network. What should you do?

A. Deploy an external HTTP(S) load balancer, configure VPC firewall rules, and move the applications onto Compute Engine virtual machines.

B. Deploy an external HTTP(S) load balancer, configure Google Cloud Armor, and move the application onto Compute Engine virtual machines.

C. Containerize the application and move it into Google Kubernetes Engine (GKE). Create a GKE service to expose the pods within the cluster, and set up a GKE network policy.

D. Containerize the application and move it into Google Kubernetes Engine (GKE). Create an internal load balancer to expose the pods outside the cluster, and configure Identity-Aware Proxy (IAP) for access.

## Feedback

A is not correct because firewall rules do not block malicious traffic into a VPC but rather block it at the VM level.

B is correct because the external HTTP(s) load balancer will improve access latency and Cloud Armor can be configured to block the Distributed Denial-of-Service (DDoS) attack.

C is not correct because a GKE service does not expose a set of pods outside of a cluster and a GKE network policy only filters traffic between pods and services.

D is not correct because a GKE internal load balancer will not load balance external traffic and anonymous users need access to the website so IAP is not a fit.

https://cloud.google.com/vpc/docs/firewalls

https://cloud.google.com/load-balancing/docs/tutorials/optimize-app-latency

https://cloud.google.com/armor/docs/security-policy-concepts

https://cloud.google.com/kubernetes-engine/docs/concepts/service

https://cloud.google.com/kubernetes-engine/docs/how-to/network-policy

https://cloud.google.com/kubernetes-engine/docs/concepts/ingress-ilb

https://cloud.google.com/iap/docs/concepts-overview#when_to_use_iap