
#THIS IS A VERY SIMPLE PROJECT ON KUBEADM WITH GCP from local machine
# my-manual-cluster-app

## Setup Instructions

1. Replace YOUR_DOCKERHUB_USERNAME inside:
   k8s/deployment.yaml

2. Add GitHub Secrets:
   - DOCKER_USERNAME
   - DOCKER_PASSWORD
   - CONTROL_PLANE_IP
   - SSH_PRIVATE_KEY (deploy key)

3. Push to main branch:
   git push origin main

CI/CD will:
- Build Docker image
- Push to DockerHub
- SSH into control plane
- Deploy to Kubernetes cluster

Access app:
http://CONTROL_PLANE_IP:30007


