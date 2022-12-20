# CI/CD Pipeline using CloudBuild & GKE
## Author - Prayag Sangode

## Diagram
![alt text] (https://cloud.google.com/static/kubernetes-engine/images/gitops-tutorial-pipeline-architecture.svg)

## Services -

- Cloud Source Repositories - Mirrored a GitHub repository to Cloud Source Repositories. With this configuration, commits that we push to the GitHub repository are copied, or mirrored, into a repository hosted in Cloud Source Repositories. 
- GKE to deploy html ap
- Artifact Registry to store docker images
- CloudBuild to build CI/CD pipeline - trigget is created
