# Rabbitmq

We use bastion host as Docker server and EKS client.
Make sure `aws configure` is done in bastion and connected to EKS cluster.

```
aws eks update-kubeconfig --region us-east-1 --name roboshop-dev
```
```
kubectl create namespace roboshop
```

```
git clone https://github.com/Lingaiahthammisetti/13.11.roboshop-rabbitmq.git
```

```
cd 13.11.roboshop-rabbitmq
```

```
helm upgrade --install rabbitmq . -n roboshop
```

```
kubectl get pods -n roboshop
```

