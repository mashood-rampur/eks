2048 App
-----------

Create Fargate profile
------------------------
```bash
eksctl create fargateprofile \
    --cluster my-eks-cluster \
    --region ap-south-1 \
    --name alb-sample-app \
    --namespace game-2048
```

Deploy the deployment, service and Ingress
----------------------------------------------
```bash
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```
