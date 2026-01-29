# Enbition Deploy

This repository contains the **deployment configurations** for the Enbition application, intended to be deployed on **OpenShift** using a GitOps-style workflow (Argo CD).

It acts as the **single source of truth for deployment**, separated from the application source code repositories.

## Purpose

The goal of this repository is to manage how Enbition microservices are:
- Deployed to OpenShift
- Configured per environment
- Updated in a controlled and reproducible way

Application code is **not** stored here. Only deployment-related manifests and configuration live in this repository.

OpenShift continuously monitors the cluster state with what is defined here.
