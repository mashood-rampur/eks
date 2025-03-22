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

![Sample Image](https://private-user-images.githubusercontent.com/43399466/258144320-93b06a9f-67f9-404f-b0ad-18e3095b7353.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDI2MjEyODksIm5iZiI6MTc0MjYyMDk4OSwicGF0aCI6Ii80MzM5OTQ2Ni8yNTgxNDQzMjAtOTNiMDZhOWYtNjdmOS00MDRmLWIwYWQtMThlMzA5NWI3MzUzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTAzMjIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwMzIyVDA1MjMwOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWViMjQyMTM4Y2JmNmNkNzZkNjg3ZDMwOTQ5M2JjNDMyOTlmYWFhOGJiYThmYzVlNTg1ZTYxZmIyNzg2Y2Q5MGUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.z4co3-dN1rPdVKNK5H2PMZF2R_aAbJTNq5EfB5srj50)
