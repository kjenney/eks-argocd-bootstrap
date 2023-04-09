# eks-argocd-bootstrap

## Terraform

1. Launch an EKS cluster
2. Create OIDC provider
3. Create IAM policy and IAM role attached to OIDC provider
4. Setup node groups with proper tags
5. Publish helm chart OCI to ECR
6. Install ArgoCD

## ArgoCD

Create application for cluster-autoscaler that uses a helm chart in ECR and the ServiceAccount connected to OIDC provider
