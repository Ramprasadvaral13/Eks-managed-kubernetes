2048 app

create fargate profile

eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048

Deploy the deployment, service and Ingress

kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml

![image](https://github.com/Ramprasadvaral13/Eks-managed-kubernetes/assets/136104228/9bbfd753-add2-4aee-a59d-c3d702dc69dc)
