# APPS MERN TO DO

Apps from https://github.com/tuanpembual/mern-todo-app

## Kubernetes Cluster
### Requirements
- AWS CLI
- Kops
- S3 Bucket
### Setup
1. aws configure, add your access keys and secret keys
2. export s3 location into variable, for example ```export KOPS_STATE_STORE=s3://kube.retiarno.my.id```
3. create variable name for cluster name, for example ```KOPS_CLUSTER_NAME=kube.retiarno.my.id``` [optional]
4. create cluster for example ``` kops create cluster --node-count=1 --node-size=t3a.small --master-size=t3a.medium --zones=ap-northeast-2a --name=${KOPS_CLUSTER_NAME} --ssh-public-key=~/.ssh/id_rsa.pub --cloud=aws```
5. validate cluster ```kops validate cluster```



