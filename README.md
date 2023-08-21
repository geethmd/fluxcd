# Visit Counter Web Application - Flux Repo

This repo contains two key pieces of the web application.

- Manifest files related to Flux
- Manifest files which build the web app

## Manifest files related to Flux

Manifest files related to the Flux system can be found under clusters/my-cluster -> flux-system folder. These manifest files created helm-controller, kustomize-controller, notification-controller, source-controller, image-automation-controller and image-reflector-controller under the EKS cluster.

## Manifest files related to web app

Manifest files related to the web app can be found under clusters/my-cluster -> manifest folder. These manifest files created a deployment with 3 pods for the web app, a service, Ingerss with class set to 'alb', ECR scan and policy verification, a cron job that runs every 6 hours to refresh ECR credentials and an ECR image update automation service to automatically update the web app image version.

## Authors

Geeth Madhusha
