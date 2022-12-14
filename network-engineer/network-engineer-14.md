# network-engineer-14

You need to create a new Cloud Router for a VPN deployment. After creating the Cloud Router, you receive an error that the Border Gateway Protocol (BGP) session failed to be established. You need to troubleshoot the problem. What should you do?

A. Review the Cloud Router logs in the Google Cloud console. Re-configure the Cloud Router with a different BGP IP peer address.

B. Review the VPN logs in the Google Cloud console. Review the VPN status messages and check the settings on your on-premises BGP router.

C. Review the VPN logs in the Google Cloud console. Delete the Cloud Router, and create a new Cloud Router with a different BGP IP address.

D. Review the Cloud Router logs in the Google Cloud console. Create a new Cloud Router. Review the VPN status messages, and check the settings on your on-premises BGP router.

## Feedback

A is not correct because reconfiguring the Cloud Router does not solve the problem.

B is correct because the Google-recommended practice is to check that the settings on your on-premises BGP router and the settings on your Cloud Router are correct.

C is not correct because deleting the Cloud Router does not solve the problem.

D is not correct because creating a new Cloud Router does not solve the problem.

https://cloud.google.com/network-connectivity/docs/router/support/troubleshooting#bgp_session_failed_to_establish

https://cloud.google.com/network-connectivity/docs/vpn/support/troubleshooting#troubleshooting-reference