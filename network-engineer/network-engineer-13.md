# network-engieer-13

You currently have several hundred Compute Engine instances running in Google Cloud. Your security officer has created a new security policy: No VMs in your cloud environment are allowed to have external (public) IP addresses. After running a report, you discover several production applications on Compute Engine instances with assigned external IP addresses. VMs must be allowed to create external outbound connections after their external IP addresses are removed, without a reduction in networking performance. What should you do?

A. Configure a proxy Compute Engine instance to access the internet.

B. Create and configure an organizational Cloud NAT policy to deny traffic to the gateway.

C. Create a new Cloud NAT gateway to maintain external access for your Compute Engine instances.

D. Create a GKE private cluster with a new Cloud NAT gateway and Cloud Router, and select the same VPC network used by your Compute Engine instances.

## Feedback

A is incorrect because using a Compute Engine instance isn’t as secure or scalable as Cloud NAT, which is designed to solve this problem.

B is incorrect because this solution allows all VMs to access the internet.

C is correct because Cloud NAT (network address translation) allows specified resources without external IP addresses to create outbound connections to the internet.

D is incorrect because creating GKE private clusters won’t provide access for your current Compute Engine VMs.

https://cloud.google.com/nat/docs/using-nat

https://cloud.google.com/blo