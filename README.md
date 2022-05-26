# Konnect GCP Kubernetes Application Marketplace Offering

## [Technical Requirements](https://cloud.google.com/marketplace/docs/partners/kubernetes/create-app-package)

- [] Your Git repository must contain a LICENSE file, which contains the open source license for the repository.
- [] Your Git repository must contain a configuration file, which deploys your app. The configuration file can be a Kubernetes YAML manifest, or a Helm chart.
  - [] The configuration must include an Application custom resource, which describes the app.
- [] All of your app's container images must be uploaded to your registry in Container Registry. Your registry must also include a deployer image, which pushes the app's configuration to the Kubernetes API when users deploy the app from Cloud Console.
- [] You must include integration tests for the app.
- [] You must include a user guide, with steps to deploy the app from the command line, configure the app, and use the app.

## User Guide

[Requirements](https://cloud.google.com/marketplace/docs/partners/kubernetes/create-app-package#user-guide)

### Overview

A general app overview, covering basic functions and configuration options. This section must also link to the published product on Google Cloud Marketplace.

### One-time setup

Configuring client tools such as kubectl or Helm. as applicable.
Installing the Application CustomResourceDefinition (CRD), so that your cluster can manage the Application resource.
If you are selling a commercial app, steps for acquiring and deploying a license Secret from Google Cloud Marketplace.

### Installation

Commands for deploying the app.
Passing parameters available in UI configuration.
Pinning image references to immutable digests.
If you add custom input fields to your deployer schema, add information about the expected values, if applicable.

Learn about adding input fields to your deployer

### Basic Usage

Connecting to an admin console (if applicable).
Connecting a client tool and running a sample command (if applicable).
Modifying usernames and passwords.
Enabling ingress and installing TLS certs (if applicable).

### Back up and restore

Backing up app state.
Restoring app state from a backup.

### Image updates

Updating the app images for patches or minor updates.

### Scaling

Scaling the app (if applicable).

### Deletion

Deleting the app.
Cleaning up any resources that might be intentionally orphaned, such as PersistentVolumeClaims.
