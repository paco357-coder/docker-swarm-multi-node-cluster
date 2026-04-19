# docker-swarm-multi-node-cluster

Built a 2-node Docker Swarm cluster using a home lab environment and managed it with Portainer. Deployed a replicated web service across multiple nodes and validated failover behavior under node failure conditions.

🧱 Architecture
PC1 (Manager) – Swarm leader node
PC2 (Worker) – Executes container workloads
Swarm cluster configured using Docker Engine
Centralized management via Portainer


⚙️ Technologies Used
Docker Engine
Docker Swarm
Portainer
NGINX (containerized web service)
Linux (Ubuntu)


🚀 Key Features
Multi-node cluster deployment
Container replication across nodes
Placement constraints (max_replicas_per_node)
Ingress networking for service exposure
Failover testing and recovery validation

🧪 Failover Testing

Simulated node failure by stopping Docker on the worker node:sudo systemctl stop docker


Observed Behavior:
Swarm detected node failure
One replica remained active on the manager node
Second replica entered pending state due to placement constraints


Demonstrated:

Distributed container orchestration
High availability concepts
Scheduler behavior under resource constraints
Real-world tradeoffs between availability and placement policies


