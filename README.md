# kubernetes-dashboard

获取dashboard image镜像、修改TAG：
docker pull registry.cn-hangzhou.aliyuncs.com/rsqlh/kubernetes-dashboard:v1.10.1
docker tag registry.cn-hangzhou.aliyuncs.com/rsqlh/kubernetes-dashboard:v1.10.1 k8s.gcr.io/kubernetes-dashboard-amd64:v1.10.1
docker rmi registry.cn-hangzhou.aliyuncs.com/rsqlh/kubernetes-dashboard:v1.10.1

创建pod：
kubectl  -n kube-system create -f .
查看pod：
kubectl get svc,pod --all-namespaces | grep dashboard
