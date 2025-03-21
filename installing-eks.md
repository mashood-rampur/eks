Install EKS
------------
Please follow the prerequisites doc before this.

Install using Fargate
---------------------

eksctl create cluster --name my-eks-cluster --region ap-south-1 --fargate

Delete the cluster
-------------------

eksctl delete cluster --name my-eks-cluster --region ap-south-1
