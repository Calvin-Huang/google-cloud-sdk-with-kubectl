# google-cloud-sdk-with-kubectl
The lightweight docker image for managing GKE.

Base on the google/cloud-sdk:alpine image, and add the kubectl as the basic tool for managing GKE, it's lightweight.

For instance, you can use this image to configure the gitlab-runner or other CI/CD environments which use the docker-machine as executor, and you're using GKE for your service/product.

It's easy to set up the kubenetes cluster in your runner which has `https://www.googleapis.com/auth/cloud-platform` scope, and the most important is, you don't need to prepare any service account credential anymore.
