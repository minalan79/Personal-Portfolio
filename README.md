# Minalan A S | DevOps & Cloud Engineering

I build and automate cloud infrastructure, delivery pipelines, and system operations. My work spans multi-account AWS environments, Terraform, CI/CD, and Linux and Windows image automation. The projects below show how I approach infrastructure delivery and Kubernetes validation.

## Featured projects

### [Kronos](https://github.com/minalan79/Kronos) · Deploying a containerized app to AKS

Kronos is an end-to-end Azure deployment project. Terraform defines the AKS infrastructure, and Azure Pipelines builds the Flask container image, provisions infrastructure, and deploys the application. The Kubernetes deployment defines readiness and liveness probes and container resource requests and limits.

| What to review | Where to start |
| --- | --- |
| How the AKS cluster is configured | [Terraform cluster definition](https://github.com/minalan79/Kronos/blob/main/terraform/azure/cluster.tf) |
| How the build, infrastructure, and deployment stages fit together | [Azure Pipelines workflow](https://github.com/minalan79/Kronos/blob/main/azure-pipelines.yml) |
| How Kubernetes checks app health and manages resource allocation | [Deployment manifest](https://github.com/minalan79/Kronos/blob/main/k8s/deployment.yaml) |

### [Kubernetes Config Validator](https://github.com/minalan79/k8s-config-validator) · Catching manifest errors before deployment

A Go CLI that checks Kubernetes YAML against version-specific schemas. It accepts files, directories, and stdin, and returns a nonzero exit code when validation fails, so it can be used as a CI check.

Start with the [usage examples and sample output](https://github.com/minalan79/k8s-config-validator#usage), then inspect the [invalid manifest fixture](https://github.com/minalan79/k8s-config-validator/blob/master/example-manifests/test-invalid.yml) to see an input the validator is designed to catch.

## Professional focus

- **AWS infrastructure and governance** — multi-account provisioning with Terraform, IAM and KMS access controls, and CI/CD with CodePipeline, CodeBuild, and Jenkins.
- **OS image and lifecycle automation** — Packer-based golden AMIs for RHEL and Windows, plus operational automation with Systems Manager and Ansible.
- **Observability** — infrastructure metrics and dashboards with CloudWatch, Prometheus, and Grafana.

[GitHub profile](https://github.com/minalan79)
