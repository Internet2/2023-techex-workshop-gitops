# Internal Lab Assets

This folder contains assets that were used to deploy the containerized Ubuntu environment for this workshop.

## Deploying the container

1. `docker build -t gitops .`
2. `docker run -dp 127.0.0.1:22:2000 gitops`