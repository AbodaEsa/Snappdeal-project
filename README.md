# Snappdeal-project
📌 Project Overview
Designed and implemented a production‑grade, scalable cloud architecture for a containerized eCommerce platform on AWS. Built a complete CI/CD pipeline integrated with Amazon ECR and deployed the application on a Kubernetes cluster with automated scaling, secure secret management, and self‑managed stateful services.

Replaced managed database and cache services with containerized PostgreSQL 17 and Redis 6.2 while maintaining high availability and performance.

✅ Key Highlights
☁️ Cloud Architecture (AWS)
Designed AWS infrastructure architecture
Integrated Amazon ECR for container image management
Implemented secure IAM-based authentication for registry access
Designed network and service isolation for production workloads
🐳 Kubernetes Architecture
Designed and deployed:
Application Deployment (4 replicas)
PostgreSQL 17 (persistent volume backed)
Redis 6.2 (in-memory caching layer)
Horizontal Pod Autoscaler (CPU & Memory based)
Configured:
Resource requests & limits
Liveness & readiness probes
Rolling updates with zero downtime
Namespace isolation
RBAC for secure automation
🔄 CI/CD Pipeline
Git-based CI pipeline builds Docker images
Images pushed automatically to AWS ECR
Kubernetes pulls images using imagePullSecrets
Implemented automated ECR token refresh CronJob (every 10 hours)
Eliminated ImagePullBackOff risks
🔐 Security & Automation
Kubernetes Secrets for sensitive credentials
IAM-based AWS authentication
RBAC-based service account for automated secret rotation
Secure container runtime practices
📈 Scalability & Resilience
Horizontal Pod Autoscaler (HPA)
Multi-replica stateless app architecture
Dedicated database and caching layer
Designed for production-grade reliability
