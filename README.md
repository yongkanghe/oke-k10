#### Follow [@YongkangHe](https://twitter.com/yongkanghe) on Twitter, Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

I just want to build an OKE Cluster (Oracle Kubernetes Engine) to play with the various Data Management capabilities e.g. Backup/Restore, Disaster Recovery and Application Mobility. 

It is challenging to create a OKE cluster if you are not familiar to it. After the OKE Cluster is up running, we still need to install Kasten, create a sample DB, create policies etc.. The whole process is not that simple.

![image](https://pbs.twimg.com/media/FSRxfp9aIAIolN2?format=jpg&name=small)

This script based automation allows you to build a ready-to-use Kasten K10 demo environment running on OKE in about 3 minutes. If you don't have an OKE Cluster, you can watch the Youtube video below and follow the guide to build an OKE cluster first. Once the OKE Cluster is up running, you can proceed to the next steps. 

# 10 mins Build a OKE cluster
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/DnERr8xMiuU/0.jpg)](https://www.youtube.com/watch?v=DnERr8xMiuU)
#### Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

# Here Are the prerequisities. 

1. Go to your terminal, download and set your kubeconfig
2. Verify if you can access the cluster via kubectl
````
kubectl get nodes
````
3. Clone the github repo, run below command
````
git clone https://github.com/yongkanghe/oke-k10.git
````
4. Install the tools and set Alibaba Cloud Access Credentials
````
cd oke-k10;./ociprep.sh
````
5. Optionally, you can customize the region, bucketname
````
vi setenv.sh
````
# To build the labs, run 
````
./k10-deploy.sh
````
1. Install Kasten K10
2. Deploy a Postgresql database
3. Create an OCI OS location profile
4. Create a backup policy for Postgresql
5. Backup jobs scheduled automatically

# To delete the labs, run 
````
./k10-destroy.sh
````
1. Remove Postgresql database
2. Remove Kasten K10
3. Remove all the relevant snapshots
4. Remove the objects from the storage bucket

# 3 mins Backup Containers on OKE
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Su9ZWZq2XG0/0.jpg)](https://wwww.youtube.com/watch?v=Su9ZWZq2XG0)
#### Subscribe [K8s Data Management](https://www.youtube.com/channel/UCm-sw1b23K-scoVSCDo30YQ?sub_confirmation=1) Youtube Channel

# Kubernetes / Kasten Learning
http://k8s.yongkang.cloud

# Earn Kubernetes Badges
https://lnkd.in/gpptXmnY

# Kasten - No. 1 Kubernetes Backup
https://kasten.io 

# Contributors
#### Follow [Yongkang He](http://yongkang.cloud) on LinkedIn, Join [Kubernetes Data Management](https://www.linkedin.com/groups/13983251) LinkedIn Group
