# splunk-operator-for-kubernetes-practice
SOK테스트 한 내용 정리

## doc

- https://github.com/splunk/splunk-operator/blob/main/docs/README.md

## minikube

- install
https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fbinary+download


```bash
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-amd64

sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64
```

- docker env

```bash
eval $(minikube docker-env)
```

## install

```bash
wget -O splunk-operator-cluster.yaml https://github.com/splunk/splunk-operator/releases/download/2.5.2/splunk-operator-cluster.yaml


kubectl apply -f splunk-operator-cluster.yaml --server-side

```

최신버전 : 2.8.1

```bash
wget -O splunk-operator-cluster.yaml https://github.com/splunk/splunk-operator/releases/download/2.8.1/splunk-operator-cluster.yaml
kubectl apply -f splunk-operator-cluster.yaml --server-side
```

## upgrade

- https://github.com/splunk/splunk-operator/blob/main/docs/SplunkOperatorUpgrade.md
