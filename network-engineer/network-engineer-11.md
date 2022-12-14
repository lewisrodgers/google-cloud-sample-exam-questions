# network-engineer-11

Your organization provides a digital streaming service in several regions worldwide. Customer feedback indicates that performance is inconsistent. You set up Cloud CDN with Cloud Storage backend buckets. You want to create the most efficient configuration to improve performance. What should you do to optimize performance?

A. Enable HTTP/3 and QUIC protocol support.

B. Use negative caching to reduce the load on your backends.

C. Configure Google Cloud Armor with WAF rules, and enable HTTP/3 and QUIC protocol support.

D. Enable HTTP/3, QUIC protocol support, and negative caching to reduce the load on your backends.

## Feedback

A is not correct because enabling HTTP/3 and QUIC protocol support alone won’t solve the performance issue.

B is not correct because, although negative caching does improve the performance, using it with

HTTP/3 and QUIC protocol support would further improve performance.

C is not correct because Google Cloud Armor rules are used to improve security, not to resolve performance issues, and enabling HTTP/3 and QUIC protocol support alone won’t solve the performance issue.

D is correct because ensuring that HTTP/3, QUIC protocol support, and negative caching are enabled and configured will optimize performance.

https://cloud.google.com/cdn/docs/best-practices?hl=en#optimize_performance