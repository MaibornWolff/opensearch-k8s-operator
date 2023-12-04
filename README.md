# OpenSearch-operator

The Kubernetes OpenSearch Operator is used for automating the deployment, provisioning, management, and orchestration of OpenSearch clusters and OpenSearch dashboards.

## Getting started

The operator can be installed easily using helm on any CNCF-certified kubernetes cluster:

The Operator can be easily installed using Helm:

1. Add the helm repo: `helm repo add opensearch-operator https://maibornwolff.github.io/opensearch-operator/`
2. Install the Operator: `helm install opensearch-operator opensearch-operator/opensearch-operator`
