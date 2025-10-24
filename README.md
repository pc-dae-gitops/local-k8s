# Template for deploying K8s Cluster

This repository contains the template for deploying a K8s cluster on a MacBook. Use this repository template to create a new repository and follow the instructions below to deploy a K8s cluster.

On a MacBook it is designed to use the Docker Kubernetes deployed from Docker Dashboard but can be used with any Kubernetes cluster.

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) (required for local cluster)
- [Kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/) (required by various scripts)
- [Flux](https://fluxcd.io/docs/installation/) (required by various scripts)
- [vault cli](https://www.vaultproject.io/docs/install) (required by various scripts)
- [jq](https://stedolan.github.io/jq/download/) (required by various scripts)
- [yq](https://mikefarah.gitbook.io/yq/) (required by various scripts)
- [openssl](https://www.openssl.org/source/) (required to generate cluster certificate)
- [direnv](https://direnv.net/docs/installation.html) (optional)

## Setup

Once you have created your own repository using this template, you will need to update the `.envrc` file with the correct values for your environment.

Start or reset the Kubernetes cluster using the Docker Dashboard.

Copy the `resources/github-secrets.sh.sample` file to `resources/github-secrets.sh` and update the values for your GitHub organization.

## Deploy

Once Flux has deployed the cluster

## Destroy

To destroy the cluster run the `reset.sh` script. This will destroy the K8s cluster.
