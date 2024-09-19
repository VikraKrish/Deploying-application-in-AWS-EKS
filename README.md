# Deploying-application-in-AWS-EKS
Deploying application in AWS EKS

**Steps to deploy application**
1.	Create the underlying infrastructure (VPC, subnets, route tables, internet gateway, nat gateway, security groups).
2.	Create EKS cluster role with policies - AmazonEKSClusterPolicy, AmazonEKSVPCResourceController.
3.	Create EKS node group role with policies - AmazonEKSWorkerNodePolicy, AmazonEC2ContainerRegistryReadOnly, AmazonEKS_CNI_Policy.
4.	Create the EKS cluster.
5.	Create the node group.
6.	Apply the deployment.yaml kubectl config.

**Some helpful commands**
1. To set kube config context
aws eks update-kubeconfig --region us-east-1 --name clusterName
2. To apply kubectl config
kubectl apply -f config.yaml
3. Add helm repo
helm repo add eks https://aws.github.io/eks-charts
helm install load balancer
helm install aws-load-balancer-controller eks/aws-load-balancer-controller -n kube-system --set clusterName=clusterName --set serviceAccount.create=false --set serviceAccount.name=aws-load-balancer-controller




<img width="895" alt="image" src="https://github.com/user-attachments/assets/3c33fb69-a441-4f79-ab6c-786400324d7a">

