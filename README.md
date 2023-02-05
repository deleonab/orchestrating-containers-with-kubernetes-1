### PROJECT: Orchestrating containers with Kubernetes PART 1

![orchestrating-containers with Kubernetes](kubernetes.png)


#### Our aim is to achieve the following:

- Install and configure master (also known as control plane) components and worker nodes (or just nodes).
- Apply security settings across the entire cluster (i.e., encrypting the data in transit, and at rest)
- In transit encryption - encrypting communications over the network using HTTPS
- At rest encryption - encrypting the data stored on a disk
- Plan the capacity for the backend data store etcd
- Configure network plugins for the containers to communicate
- Manage periodical upgrade of the cluster
- Configure observability and auditing

#### Tools to be used 

- VM: AWS EC2
- OS: Ubuntu 20.04 lts+
- Docker Engine
- kubectl console utility
- cfssl and cfssljson utilities
- Kubernetes cluster
- We shall create 3 EC2 Instances, and in the end, we will have the following parts of the cluster properly configured:

#### Final Outcome 
- One Kubernetes Master
- Two Kubernetes Worker Nodes
- Configured SSL/TLS certificates for Kubernetes components to communicate securely
- Configured Node Network
- Configured Pod Network