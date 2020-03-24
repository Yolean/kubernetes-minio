
# Minio on Kubernetes using Kustomize

We used Helm for our first generation Minio hosting.
That was just a layer of obscurity that we didn't need,
so we quickly switched to maintaining the actual yaml.

We used Minio's operator for our second generation Minio hosting.
That turned out to be harder to operate than minio itself.
We never knew when an instance change would propagate to pods.

This is our third attempt. Plain old yaml, but with Kustomize.
