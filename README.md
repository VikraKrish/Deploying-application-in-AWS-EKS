# Deploying-application-in-AWS-EKS
Deploying application in AWS EKS
<img width="895" alt="image" src="https://github.com/user-attachments/assets/3c33fb69-a441-4f79-ab6c-786400324d7a">


**Steps to deploy the application in EKS**
Create the underlying infrastructure (VPC, subnets, route tables, internet gateway, nat gateway, security groups).
Create EKS cluster role with policies - AmazonEKSClusterPolicy, AmazonEKSVPCResourceController.
Create EKS node group role with policies - AmazonEKSWorkerNodePolicy, AmazonEC2ContainerRegistryReadOnly, AmazonEKS_CNI_Policy.
Create the EKS cluster.
Create the node group.
Apply the deployment.yaml kubectl config.
