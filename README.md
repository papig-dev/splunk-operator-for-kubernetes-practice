# splunk-operator-for-kubernetes-practice
SOK테스트 한 내용 정리

## doc

- https://github.com/splunk/splunk-operator/blob/main/docs/README.md

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
