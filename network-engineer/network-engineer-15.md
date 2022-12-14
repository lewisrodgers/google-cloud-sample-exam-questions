# network-engineer-15

Your network administrator has created several HA VPNs in Google Cloud. However, several applications that use the HA VPN are demonstrating a delayed response at unexpected times. You need to troubleshoot the problem. What should you do?

A. Analyze the Google Cloud Console logs and Network Topology information.

B. Use Performance Dashboard to review the packet loss and latency metrics.

C. Use Performance Dashboard and perform a Connectivity Test to detect configuration issues.

D. Reconfigure your current HA VPN with FOUR_IPS_REDUNDANCY, and perform benchmark testing.

## Feedback

A is not correct because it's the wrong place to look for the information you need to troubleshoot.

B is correct because to identify any latency or packet loss issues, you can monitor the performance of the entire Google Cloud network. In the Google Cloud performance view, Performance Dashboard shows packet loss and latency metrics across all of Google Cloud resources.

C is not correct because performing a connectivity test only detects configuration issues. It does not try to send packets through the data plane to verify connectivity.

D is not correct because reconfiguring your HA VPN does not identify the problem.

https://cloud.google.com/network-connectivity/docs/vpn/support/troubleshooting#network_latency_issues_between_vms_in_different_regions

https://cloud.google.com/network-intelligence-center/docs/performance-dashboard/how-to/using-performance-dashboard