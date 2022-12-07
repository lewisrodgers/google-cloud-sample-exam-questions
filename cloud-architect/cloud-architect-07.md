# cloud-architect-07

For this question, refer to the [Mountkirk Games case study](https://services.google.com/fh/files/blogs/master_case_study_mountkirk_games.pdf).

You need to implement Virtual Private Cloud (VPC) Service Controls for Mountkirk Games. Mountkirk Games wants to allow Cloud Shell usage by its developers. Developers should not have full access to managed services. You need to balance these conflicting goals with Mountkirk Games’ business requirements. What should you do?

A. Use VPC Service Controls for the entire platform.

B. Prioritize VPC Service Controls implementation over Cloud Shell usage for the entire platform.

C. Include all developers in an access level associated with the service perimeter, and allow them to use Cloud Shell.

D. Create a service perimeter around only the projects that handle sensitive data, and do not grant your developers access to it.


## Feedback

A is not correct because VPC Service Controls do not directly affect scaling of Google Cloud architecture.

B is not correct because a security perimeter is not a business requirement, but rapid iteration is.

C is not correct because it works but does not scale, and we do not want to give users this much access.

D is correct because VPC Service Controls protects data, and Cloud Shell facilitates rapid iteration of Google Cloud architecture changes.

https://cloud.google.com/vpc-service-controls/docs/supported-products#shell

https://cloud.google.com/vpc-service-controls