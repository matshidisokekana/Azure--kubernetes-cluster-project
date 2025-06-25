
# 🚀 Deploying a Public Docker Image to Azure Container Apps

This project demonstrates how to **deploy a Docker container image** (MongoDB:1.27) from **Docker Hub** to **Azure Container Apps** using the Azure Portal. The deployment replicates local behavior in the cloud with minimal setup.

---

## 🛠️ Tools Used

- Azure Portal
- Docker Hub (public image)
- Azure Container Apps
- Azure Resource Group + Container Environment

---

## 🔧 Project Steps

1. **Create a Resource Group**
   - Name: `MongoAppRG`

2. **Create Container App Environment**
   - Region: `East US` (or as required)
   - Container App Environment: `MongoAppEnv`

3. **Configure App**
   - Name: `mongo-container-app`
   - Image Source: **Docker Hub**
   - Image: `mongo:1.27`
   - Port: `80`  
   - Ingress: **Enabled** (Allow public access)
   - CPU/Memory: `0.5 CPU / 1.0 GiB`

4. **Deploy**
   - Click **Review + Create**, then **Create**
   - After deployment, open the **Resource URL** – your app runs in the cloud exactly as it did locally

---

## 🌟 What I Gained & Why It Matters

### 🔍 What I Learned

- Gained **hands-on experience** in deploying container images directly to **Azure Container Apps**, simulating real-world cloud deployments.
- Understood how to configure container settings (like ports and tags) through the **Azure Portal**, improving cloud app readiness.
- Learned the **value of public image repositories** (Docker Hub) and how Azure can securely and quickly pull and deploy these images.

### 💡 Why Azure Container Apps?

- **Fast Deployment**: Azure enables near-instant deployment of containers without needing to manage infrastructure or write orchestration scripts.
- **Scalable & Lightweight**: It’s ideal for testing microservices and running small workloads that don't require full Kubernetes complexity.
- **Cost-Efficient**: Serverless container hosting reduces cost and avoids overprovisioning.
- **Cloud-Native Ready**: Builds real-world skills applicable to production environments, CI/CD pipelines, and DevOps automation.

This project helped me develop a **cloud-native mindset**, preparing me for larger-scale deployments using ACR, GitHub Actions, and AKS in future projects.

---

## 📸 Result

- ✅ MongoDB container successfully deployed from Docker Hub
- 🌐 Accessible via Azure-generated **resource URL**
- ⚡ Quick and efficient deployment, simulating real-world container hosting

---

## 📁 Folder Structure

```

docker-to-azure-container-app/
├── README.md
└── (Azure deployment was portal-based; no local source files needed)
## 🙋🏽‍♂️ Author

**Matshidis0**

---



