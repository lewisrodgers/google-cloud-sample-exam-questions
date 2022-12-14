# network-engineer-01

You have a global secure web application hosted on a Compute Engine unmanaged instance group. The application is currently deployed in us-central1-a. However, due to company growth, most of your new customers are geographically closer to the europe-west2 region. You need to implement a solution that allows the application to automatically scale to meet the demand for future customers and also follows Google-recommended practices. What should you do?

A. Deploy a network load balancer with a regional virtual IP address. Configure a backend with a managed instance group.

B. Deploy an HTTP(S) load balancer with a regional virtual IP address. Configure a backend with a managed instance group.

C. Deploy an HTTP(S) load balancer with a global virtual IP address. Configure a backend in europe-west2-a with a managed instance group.

D. Deploy a network load balancer with a global virtual IP address. Configure a backend in europe-west2-a with an unmanaged instance group.

## Feedback

A is incorrect because you can’t serve customers in multiple regions by using only a network load balancer.

B is incorrect because a regional HTTP load balancer only supports one region, so you can’t serve customers in multiple regions.

C is correct because it follows Google-recommended practices. A global load balancer directs traffic across multiple regions through a single IP address. By using both of these services to distribute your application across multiple zones, you can help ensure that your application is available even in extreme cases, like a zonal disruption.

D is incorrect because a network load balancer is regional, not global, so it is not a good choice for global HTTPS applications.

https://cloud.google.com/load-balancing/docs/https/use-cases#cross-region_load_balancing

https://cloud.google.com/compute/docs/tutorials/high-availability-load-balancingt
