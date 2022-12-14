# network-engineer-02

Your company has a regional Compute Engine software as a service (SaaS) application that currently allows traffic from the entire internet. The application should not be accessible from the public internet. You also want to allow only certain virtual machines (VMs) to access your application by using Secure Shell (SSH). What should you do to satisfy the requirements?

A. Delete the rule that allows traffic from 0.0.0.0/0. Create a firewall rule to allow traffic from 192.168.0.0/16, 172.16.0.0/12, and 10.0.0.0/8.

B. Create a new rule that denies traffic from 0.0.0.0/0. Create a firewall rule to deny traffic from 192.168.0.0/16, 172.16.0.0/12, and 10.0.0.0/8.

C. Delete the prepopulated rule that allows SSH traffic from 0.0.0.0/0. Create a network tag that allows access to TCP 22, and apply the tag to each VM that will access the application.

D. Delete the prepopulated rule that allows SSH traffic from 0.0.0.0/0. Create a network tag that allows access to TCP 3389, and apply the newly created tag to each VM that will access the application.

## Feedback

A is incorrect because creating a new rule that allows traffic from 0.0.0.0/0 would allow public access to the application.

B is incorrect because those firewall rules would deny both public and private access.

C is correct because using a network tag with access to TCP 22 allows access to Secure Shell and lets you permit access from specific Virtual Private Clouds (VPCs).

D is incorrect because TCP 3389 is used for the Remote Desktop Protocol (RDP).

https://cloud.google.com/vpc/docs/firewalls