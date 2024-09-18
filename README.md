# Deploying-application-in-AWS-EKS
Deploying application in AWS EKS

**Steps to deploy the application in EKS**
1.Create the underlying infrastructure (VPC, subnets, route tables, internet gateway, nat gateway, security groups).
2.Create EKS cluster role with policies - AmazonEKSClusterPolicy, AmazonEKSVPCResourceController.
3.Create EKS node group role with policies - AmazonEKSWorkerNodePolicy, AmazonEC2ContainerRegistryReadOnly, AmazonEKS_CNI_Policy.
4.Create the EKS cluster.
5.Create the node group.
6. Apply the deployment.yaml kubectl config.

<img width="895" alt="image" src="https://github.com/user-attachments/assets/3c33fb69-a441-4f79-ab6c-786400324d7a">

