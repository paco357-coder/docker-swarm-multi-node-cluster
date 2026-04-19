# Docker Swarm Multi-Node Cluster

## 📌 Project Overview
Built a 2-node Docker Swarm cluster using a home lab environment and managed it with Portainer. Deployed a replicated web service across multiple nodes and validated failover behavior under node failure conditions.

---

## 🧱 Architecture

- **PC1 (Manager)** – Swarm leader node  
- **PC2 (Worker)** – Executes container workloads  
- Docker Swarm cluster with centralized management  

---

## ⚙️ Technologies Used

- Docker Engine  
- Docker Swarm  
- Portainer  
- NGINX  
- Linux (Ubuntu)  

---

## 🚀 Key Features

- Multi-node cluster deployment  
- Container replication across nodes  
- Placement constraints (`max_replicas_per_node`)  
- Ingress networking  
- Failover testing  

---

## 🧪 Failover Testing

Simulated node failure:

```bash
sudo systemctl stop docker
Observed Behavior:
