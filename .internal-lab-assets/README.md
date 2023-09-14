# Internal Lab Assets

This folder contains assets that were used to deploy the containerized Ubuntu environment for this workshop. It is used by presenters and is also included for any curious minds.

## Deploying the container

From the host, gitops-tx23-workshop.macc.ns.internet2.edu:

1. `cd /lab-gitops/2023-techex-workshop-gitops/internal-lab-assets`
2. `docker build -f Containerfile -t gitops .`
3. `docker run --hostname gitops -t -i -dp :2431:22 gitops`

User SSH is now available via `ssh gitops-tx23-workshop.macc.ns.internet2.edu -p 2431`
