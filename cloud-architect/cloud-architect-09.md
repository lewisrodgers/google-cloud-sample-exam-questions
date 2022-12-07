# cloud-architect-09

For this question, refer to the [Helicopter Racing League (HRL) case study](https://services.google.com/fh/files/blogs/master_case_study_helicopter_racing_league.pdf).

HRL wants you to help them bring existing recorded video content to new fans in emerging regions. Considering the HRL business and technical requirements, what should you do?

A. Serve the video content directly from a multi-region Cloud Storage bucket.

B. Use Cloud CDN to cache the video content from HRL’s existing public cloud provider.

C. Use Apigee Edge to cache the video content from HRL’s existing public cloud provider.

D. Replicate the video content in Google Kubernetes Engine clusters in regions close to the fans.

## Feedback

A is not correct because a multi-region bucket does not serve all global areas with similar latency.

B is correct because Cloud CDN can be used to cache data hosted on other cloud providers and supports large objects such as video.

C is not correct because Apigee Edge is not designed to cache data larger than 512 KB.

D is not correct because replicating the video content introduces unnecessary complexity.

https://cloud.google.com/storage/docs/locations#considerations

https://cloud.google.com/cdn/docs/caching#maximum-size

https://cloud.google.com/cdn/docs/custom-origins-overview#hybrid_and_multi-cloud_architectures

https://docs.apigee.com/api-platform/antipatterns/caching-large

https://cloud.google.com/solutions/building-a-multi-cluster-service-mesh-on-gke-using-replicated-control-plane-architecture