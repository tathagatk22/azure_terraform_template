# azure_terraform_template

This repository holds the Terraform template for Cluster creation on Azure Kubernetes Service.

#### Using Jenkinsfile

1. Using Jenkins file user can provide all the required details to create the new Kubernetes Cluster on Azure using Terraform.
2. This new Kubernetes cluster's kube_config_raw is visible on the Jenkins Output and is saved in Jenkins Server for further resource deployment using existing Jenkins Server.

#### Using Terraform

User can fill all the appropriate values in terraform.tfvars and perform the below steps.

```
$ terraform init
$ terraform plan
$ terraform apply --auto-approve
$ terraform output kube_config
```

User can use this kube_config to further deployment of the resources.