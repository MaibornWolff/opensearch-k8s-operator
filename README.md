# OpenSearch Kubernetes Operator

**This is a fork of the [opensearch-k8s-operator](https://github.com/opensearch-project/opensearch-k8s-operator) that was formerly hosted by [Opster](https://opster.com) and is now part of the opensearch-project. Due to confusion and instability in the project, MaibornWolff has decided to (temporarily) provide a fork of the operator with compatible and stable releases. Feel free to open an issue or start a discussion if you have questions.**

The Kubernetes OpenSearch Operator is used for automating the deployment, provisioning, management, and orchestration of OpenSearch clusters and OpenSearch dashboards.

## Getting started

The Operator can be easily installed using helm on any CNCF-certified Kubernetes cluster. Please refer to the [User Guide](./docs/userguide/main.md) for installation instructions.

## Current feature list

- [x] Deploy a new OS cluster.
- [x] Ability to deploy multiple clusters.
- [x] Spin up OS dashboards.
- [x] Configuration of all node roles (master, data, coordinating..).
- [x] Scale the cluster resources (manually), per nodes' role group.
- [x] Drain strategy for scale down.
- [x] Version updates.
- [x] Change nodes' memory allocation and limits.
- [x] Secured installation features.
- [x] Certificate management.
- [x] Rolling restarts - through API.
- [x] Scaling nodes' disks - increase disk size.
- [x] Cluster configurations and nodes' settings updates.
- [x] Operator Monitoring, with Prometheus and Grafana.

## Installation

The Operator can be easily installed using Helm:

1. Add the helm repo: `helm repo add opensearch-operator https://maibornwolff.github.io/opensearch-operator/`
2. Install the Operator: `helm install opensearch-operator opensearch-operator/opensearch-operator`

## Compatibility

The opensearch k8s operator aims to be compatible to all supported opensearch versions. Please check the table below for details:

| Operator Version | Min Supported Opensearch Version | Max supported Opensearch version | Comment |
|------------------|----------------------------------|----------------------------------|---------|
| 2.5              | 1.0                              | 2.11                             |         |
| 2.4              | 1.0                              | 2.8                              |         |
| 2.3              | 1.0                              | 2.8                              |         |
| 2.2              | 1.0                              | 2.5                              |         |
| 2.1              | 1.0                              | 2.3                              |         |
| 2.0              | 1.0                              | 2.3                              |         |
| 1.x              | 1.0                              | 1.x                              |         |
| 0.x              | 1.0                              | 1.x                              | Beta    |

This table only lists versions that have been explicitly tested with the operator, the operator will not prevent you from using other versions. Newer minor versions (2.x) not listed here generally also work but you should proceed with caution and test it out in a non-production environment first.

## Development

If you want to develop the operator, please see the separate [developer docs](./docs/developing.md).

## Contributions

We welcome contributions! See how you can get involved by reading [CONTRIBUTING.md](./CONTRIBUTING.md).
