# terraform

The Terraform code required to provision an EKS cluster along with the prerequisites for running cluster-autoscaler as well as ArgoCD for deploying cluster-autoscaler.

Replace MY.IP.ADDRESS with the IP address you are using to connect to the EKS cluster:

```
terraform init
terraform plan -var="eks_endpoint_ip=MY.IP.ADDRESS"
terraform apply -var="eks_endpoint_ip=MY.IP.ADDRESS"
```
