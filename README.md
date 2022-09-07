# Terraform Kubernetes ArgoCD Bootstrap

Terraform module that installs [Argo CD](https://github.com/argoproj/argo-cd) and [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets) in a Kubernetes cluster to make it GitOps ready.

## Instructions

Using [variables.tf](./variables.tf) as reference, create a Terraform `*.tfvars` file to provide values to variables for your deployment.

Bootstrap the Kubernetes cluster for GitOps by running
```
terraform apply -var-file=<.tfvars file> -auto-approve
```
