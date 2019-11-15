# rook
rook 存储管理工具

### 安装步骤：

#### 1.使用helm
git clone https://github.com/rook/rook.git

cd rook/cluster/charts

helm install --namespace rook-ceph --name rook-ceph rook-ceph的目录

#### 2. 创建集群
git clone https://github.com/rook/rook.git

cd rook/cluster/examples/kubernetes/ceph

kubectl apply -f cluster.yaml  # 注意关于 node信息的配置

kubectl apply -f srotageclass.yaml  #创建存储类StorageClass

kubectl apply -f toolbox.yaml  #创建管理工具
