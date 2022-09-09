# Metric server is required for Horizontal Pod Autoscaler

## What is Metric Server?
```sh
It collects metrics like CPU, memory or Disk IO consumption for containers or nodes, from the Summary API, exposed by Kubelet on each node.
```

각 노드에서 Kubelet에 의해 노출되는 요약 API에서 컨테이너 또는 노드에 대한 CPU, 메모리 또는 디스크 IO 소비와 같은 메트릭을 수집합니다.

## Enable 4443 port on Master and Worker Nodes
```sh
4443
```
## Clone Metric-server helm chart on K8 Master
```sh
git clone https://github.com/prawinkorvi/metric-server.git
```

## Create Metric Server
```sh
kubectl create -f .
kubectl top pods
kubectl top nodes
```
