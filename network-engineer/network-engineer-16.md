# network-engineer-16

You need to create a new Cloud Router to connect your on-premises network to Google Cloud. You want to ensure that no services will be disrupted if you have a link failure. What should you do?

A. Enable graceful restart on your on-premises BGP device.

B. Create your Cloud Router with global dynamic routing enabled.

C. Create your Cloud Router with regional dynamic routing enabled.

D. Modify the base advertised route priority in your existing BGP session.

## Feedback

A is correct because Google-recommended practice is to enable graceful restart on your on-premises BGP device. With graceful restart, traffic between networks isn't disrupted if a Cloud Router or on-premises BGP device fails but the BGP session is re-established within the graceful restart period.

B is not correct because global dynamic routing will not prevent service disruption if a link fails.

C is not correct because regional dynamic routing will not prevent service disruption if a link fails.

D is not correct because disabling graceful restart would allow packets to drop, which would disrupt the network.

https://cloud.google.com/network-connectivity/docs/router/concepts/best-practices

https://cloud.google.com/network-connectivity/docs/router/concepts/overview#route-advertisement-default