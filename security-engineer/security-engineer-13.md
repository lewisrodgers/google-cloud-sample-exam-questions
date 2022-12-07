# security-engineer-13

Your company is deploying their applications on Google Kubernetes Engine. You want to follow Google-recommended practices. What should you do to ensure that the container images used for new deployments contain the latest security patches?

A. Use Google-managed base images for all containers.

B. Use Container Analysis to detect vulnerabilities in images.

C. Use an update script as part of every container image startup.

D. Use exclusively private images in Container Registry.

## Feedback

A is correct because Managed base images are base container images that are automatically patched by Google for security vulnerabilities, using the most recent patches available from the project upstream (for example, GitHub).

B is not correct because Container Analysis does not patch the images.

C is not correct because while an update script may help patch on startup, this will significantly increase the amount of time it takes for the instance to become ready for serving workloads.

D is not correct because private images also go out of date and need to be patched manually by the customer.

https://cloud.google.com/container-registry/docs/managed-base-images