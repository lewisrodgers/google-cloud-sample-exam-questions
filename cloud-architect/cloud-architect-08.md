# cloud-architect-08

For this question, refer to the [Mountkirk Games case study](https://services.google.com/fh/files/blogs/master_case_study_mountkirk_games.pdf).

Your new game running on Google Cloud is in public beta, and you want to design meaningful service level objectives (SLOs) before the game becomes generally available. What should you do?

A. Define one SLO as 99.9% game server availability. Define the other SLO as less than 100-ms latency.

B. Define one SLO as service availability that is the same as Google Cloud's availability. Define the other SLO as 100-ms latency.

C. Define one SLO as 99% HTTP requests return the 2xx status code. Define the other SLO as 99% requests return within 100 ms.

D. Define one SLO as total uptime of the game server within a week. Define the other SLO as the mean response time of all HTTP requests that are less than 100 ms.

## Feedback

A is incorrect because it doesn't clearly define how to measure both the availability and latency.

B is incorrect because Google Cloud availability has an impact on customer availability but it is only one factor. Also, for different Google Cloud products, the availability could be different.

C is correct because it clearly defines the service level indicators and how to measure them.

D is incorrect because there is no objective for the server uptime.

https://landing.google.com/sre/workbook/chapters/implementing-slos/
