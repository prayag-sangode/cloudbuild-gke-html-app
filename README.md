# CI/CD Pipeline using CloudBuild & GKE
## Author - Prayag Sangode

## Diagram

<img src="https://github.com/prayag-sangode/cloudbuild-gke-html-app/blob/main/cloud-build-gke.PNG" alt="Alt text" title="CI/CD Pipeline using CloudBuild & GKEe">

## Services -

- Cloud Source Repositories - Mirrored a GitHub repository to Cloud Source Repositories. With this configuration, commits that we push to the GitHub repository are copied, or mirrored, into a repository hosted in Cloud Source Repositories. 
- GKE to deploy html app
- Artifact Registry to store docker images
- CloudBuild to build CI/CD pipeline - trigger is created

## Create GKE Cluster
```sh
gcloud container clusters create gke-cluster --num-nodes 1 --zone "asia-south1-b"
gcloud container clusters list
```

## Create Artifact Registry
```sh
gcloud artifacts repositories create apps-repo --repository-format=docker --location=asia-south1-b --description="Docker repository for html app"
gcloud artifacts repositories list
```
