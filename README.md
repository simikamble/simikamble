<div align="center">

<!-- HERO HEADER BANNER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1b2a,30:1b263b,70:005a9c,100:0078d4&height=250&section=header&text=SIMRAN%20KAMBLE&fontSize=46&fontAlignY=36&desc=DevOps%20Engineer%20(3%2B%20Years)%20%7C%20Azure%20Cloud%20%7C%20CI%2FCD%20%7C%20Kubernetes%20%7C%20Terraform&descAlignY=58&descSize=18&fontColor=ffffff" width="100%" alt="Simran Kamble Header" />

# ⚡ Simran Kamble
### **DevOps Engineer | Azure Cloud Infrastructure | CI/CD Automation | Kubernetes & Docker**

<p align="center">
  <em>Hands-on DevOps Engineer with 3+ years of experience building, deploying, and maintaining resilient Microsoft Azure cloud infrastructure, automated CI/CD pipelines (Azure DevOps & GitHub Actions), Terraform IaC, and supporting 100+ application cloud migrations across Dev, UAT, and Production environments.</em>
</p>

<!-- SOCIAL & PROFESSIONAL BADGES -->
<p align="center">
  <a href="https://linkedin.com/in/simran-kamble">
    <img src="https://img.shields.io/badge/LINKEDIN-SIMRAN%20KAMBLE-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:simrankamble@example.com">
    <img src="https://img.shields.io/badge/EMAIL-GET%20IN%20TOUCH-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/simikamble">
    <img src="https://img.shields.io/badge/GITHUB-simikamble-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="#-technical-skills-ecosystem">
    <img src="https://img.shields.io/badge/ROLE-DEVOPS%20ENGINEER%20(3%2B%20YRS)-2EA44F?style=for-the-badge&logo=azure-pipelines&logoColor=white" alt="Role" />
  </a>
</p>

<!-- QUICK PILL BADGES -->
<p align="center">
  <img src="https://img.shields.io/badge/Experience-3%2B%20Years-blue?style=flat-square&logo=clock&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloud-Microsoft%20Azure-0089D6?style=flat-square&logo=microsoftazure&logoColor=white" />
  <img src="https://img.shields.io/badge/CI%2FCD-Azure%20DevOps%20%26%20GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Containers-Kubernetes%20(AKS)%20%26%20Docker-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/IaC-Terraform%20Modular-7B42BC?style=flat-square&logo=terraform&logoColor=white" />
  <img src="https://img.shields.io/badge/Governance-Azure%20Policy%20%26%20CAF-0078D7?style=flat-square&logo=azuredevops&logoColor=white" />
  <img src="https://img.shields.io/badge/FinOps-Cost%20Optimization-brightgreen?style=flat-square&logo=googlecloud&logoColor=white" />
</p>

---

</div>

## 📌 Professional Summary

Enthusiastic and hands-on **DevOps Engineer** with **3+ years of experience** specializing in **Microsoft Azure cloud infrastructure provisioning & maintenance**, **CI/CD pipeline engineering**, **containerization (Docker & Kubernetes AKS)**, and **Infrastructure as Code (Terraform)**.

Proven hands-on experience supporting large-scale enterprise initiatives, including the **cloud migration of 100+ multi-tier applications** from On-Premises Datacenters to Azure across **Dev, UAT, and Production** subscriptions. Adept at implementing secure **Hub-and-Spoke virtual networks**, automated **Terraform modules with remote state and drift detection**, shift-left security scans in pipelines, and driving **FinOps cost optimization** while ensuring high availability and compliance.

### 🎯 Key Hands-on Competencies
- ☁️ **Azure Cloud Infrastructure**: Provisioning and managing multi-subscription Azure environments aligned with Microsoft Cloud Adoption Framework (CAF) guidelines.
- 🔁 **CI/CD Automation**: Creating end-to-end multi-stage build, test, and release pipelines using **Azure DevOps (Pipelines, Repos)** and **GitHub Actions**.
- 🛠️ **Infrastructure as Code**: Developing reusable, modular **Terraform** templates with remote backend state locking, least-privilege RBAC, and pipeline drift detection.
- 🐳 **Containers & Kubernetes (AKS)**: Containerizing applications with **Docker**, deploying and managing **Azure Kubernetes Service (AKS)** clusters with ingress controllers and Secrets Store CSI.
- 🚀 **100+ App Cloud Migration Support**: Executing discovery, pre-checklists, cutover sync, and post-migration validation for 100+ workloads across Dev, UAT, and Prod.
- 🔒 **Cloud Security & Governance**: Enforcing Azure Policy, RBAC groups, Microsoft Entra ID user/group management, and Defender for Cloud recommendations.
- 💰 **FinOps & Cost Optimization**: Implementing automated VM start/stop schedules, cleaning up unattached disks/orphaned resources, and optimizing Reserved Instances.
- 🔄 **High Availability & BCDR**: Configuring VMSS, LRS/ZRS/GRS storage redundancy, Azure Backup, and Azure Site Recovery (ASR) to meet target RTO/RPO SLAs.

---

## 🏛️ Azure Cloud Architecture & CAF Landing Zones

Hands-on implementation of structured multi-subscription landing zones aligned with the **Microsoft Cloud Adoption Framework (CAF)** lifecycle: **Plan ➔ Ready ➔ Adopt ➔ Govern ➔ Secure ➔ Manage**.

### 1. Management Group & Tenant Hierarchy
```mermaid
graph TD
    Root["🏢 Tenant Root Group (Microsoft Entra ID)"]
    
    Root --> Platform["📁 Platform Management Group"]
    Root --> LandingZones["📁 Application Landing Zones (Workloads)"]
    Root --> Sandbox["📁 Sandbox Management Group"]
    Root --> Decom["📁 Decommissioned Management Group"]
    
    Platform --> SubIdentity["🔑 Identity Subscriptions (Entra ID, Key Vault)"]
    Platform --> SubConnectivity["🌐 Connectivity Subscriptions (Hub VNet, Firewall, VPN/ER)"]
    Platform --> SubManagement["📊 Management Subscriptions (Azure Monitor, LAW)"]
    
    LandingZones --> SubDev["🧪 Dev Subscription (Development Workloads)"]
    LandingZones --> SubUAT["🔬 UAT Subscription (Staging & QA)"]
    LandingZones --> SubProd["🚀 Production Subscription (High SLA Workloads)"]
    
    Sandbox --> SubPOC["🧪 Sandbox / POC Subscriptions (Budget-Capped)"]
    Decom --> SubArchive["📦 Decommissioned Subscriptions (Quarantine)"]
```

### 2. Tenant Hierarchy & Governance Best Practices
| Area | Implementation Details | Key Benefits |
| :--- | :--- | :--- |
| **Subscription Boundaries** | Segregated platform services from application landing zones across Dev, UAT, and Prod. | Reduced blast radius and clear environment isolation. |
| **Microsoft Entra ID & RBAC** | Configured security groups, user permissions, and role assignments mapped via Entra ID groups. | Principle of Least Privilege (PoLP); avoids individual user role clutter. |
| **Azure Policy & Initiatives** | Applied built-in and custom policy initiatives (e.g., allowed regions, mandatory tags, secure transfer). | Automated guardrails blocking non-compliant resource deployments. |
| **Policy Exemptions** | Documented business justifications, expiration dates, and tracked policy exemption scopes. | Controlled exceptions without compromising overall compliance posture. |
| **Subscription Lifecycle** | Standardized subscription onboarding and decommissioning procedures. | Fast workspace provisioning and safe cleanup of legacy assets. |

---

## 🌐 Hub-and-Spoke Networking Model

Hands-on design and maintenance of secure enterprise network connectivity connecting on-premises datacenters to Azure.

```mermaid
flowchart LR
    subgraph OnPrem["🏢 On-Premises Datacenter"]
        DCWorkloads["Core Systems / CIDR Assessment"]
    end

    subgraph AzureHub["🌐 HUB VNet (Centralized Inspection & Shared Services)"]
        direction TB
        GW["VPN Gateway / ExpressRoute"]
        AzFW["🛡️ Azure Firewall (UDR Central Inspection)"]
        Bastion["🔒 Azure Bastion"]
        DNSZones["📑 Private DNS Zones"]
    end

    subgraph SpokeDev["🧪 Spoke VNet: Dev"]
        DevVMs["Dev Apps / AKS Subnet"]
        DevPE["Private Endpoints"]
    end

    subgraph SpokeUAT["🔬 Spoke VNet: UAT"]
        UATVMs["UAT Services / Apps"]
        UATPE["Private Endpoints"]
    end

    subgraph SpokeProd["🚀 Spoke VNet: Production"]
        ProdAKS["Production AKS Cluster"]
        ProdData["Azure SQL / Data Services"]
        ProdPE["Private Endpoints"]
    end

    DCWorkloads <-->|"ExpressRoute / S2S VPN"| GW
    GW --> AzFW
    AzFW <-->|"VNet Peering & UDR (0.0.0.0/0)"| SpokeDev
    AzFW <-->|"VNet Peering & UDR (0.0.0.0/0)"| SpokeUAT
    AzFW <-->|"VNet Peering & UDR (0.0.0.0/0)"| SpokeProd
```

### Network Engineering Highlights
- **IP Address Management (IPAM) & CIDR Assessment**: Reviewed on-premises CIDR ranges to ensure non-overlapping address allocations for cloud VNets.
- **Hub VNet Setup**: Configured ExpressRoute/VPN Gateways, Azure Firewall, Azure Bastion, and centralized Private DNS Zones.
- **Spoke Peering & User Defined Routes (UDR)**: Configured bidirectional VNet peering and route tables routing `0.0.0.0/0` outbound traffic through Azure Firewall for centralized traffic inspection.
- **Private Endpoints**: Linked PaaS services (Azure Storage, Key Vault, Azure SQL, ACR) through Private Endpoints with Private DNS integration to eliminate internet exposure.
- **Controlled Egress**: Defined network and application firewall rules to restrict outbound traffic to approved FQDNs and ports.

---

## ⚡ DevSecOps & Infrastructure as Code (IaC)

### 1. Terraform Landing Zone Automation & Best Practices
- **Remote State Management**: Configured Azure Blob Storage backend with state locking (blob lease), encryption at rest, and strict RBAC access controls.
- **Reusable Modular Code**: Developed parameterized, modular Terraform code for VNets, subnets, NSGs, AKS, Storage Accounts, and VMSS.
- **Automated Quality & Security Checks**:
  - Code formatting and validation (`terraform fmt`, `terraform validate`, `tflint`).
  - Shift-left security scans using `tfsec` and `trivy` to detect vulnerabilities early.
  - Secret scanning with `GitGuardian` pre-commit and pipeline hooks.
  - Cost visibility using `Infracost` to estimate infrastructure changes on pull requests.
- **Pipeline Drift Detection**: Configured scheduled Azure DevOps / GitHub Actions pipelines running `terraform plan -detailed-exitcode` to detect portal out-of-band drifts.

### 2. CI/CD Pipeline Lifecycle (Azure DevOps & GitHub Actions)
```mermaid
sequenceDiagram
    autonumber
    actor Dev as DevOps Engineer / Developer
    participant Git as Azure Repos / GitHub (Trunk)
    participant Sec as Linter & Security Scans
    participant Cost as Infracost Engine
    participant Review as Reviewer / Approver
    participant Pipe as CI/CD Pipeline Runner
    participant Cloud as Microsoft Azure Infrastructure

    Dev->>Git: Short-Lived Feature Branch + Pull Request
    Git->>Sec: Automated PR Trigger: TFLint, Trivy & Secret Scanning
    Sec->>Cost: Run Infracost & Post PR Comment
    Cost->>Dev: Cost Delta Feedback on PR
    Git->>Review: Peer Review (Mandatory PR Approval, Code Owners)
    Review->>Git: Approved & Merged to Main (No Direct Push / No Delete Main)
    Git->>Pipe: Trigger Pipeline Templates: Validate & Test | Build
    Pipe->>Pipe: Run Terraform Plan across Dev/UAT/Prod Matrix
    Pipe->>Review: Manual Approval Gate for Prod Apply
    Review->>Pipe: Approved
    Pipe->>Cloud: Terraform Apply / Automated Rollback on Failure
    Note over Cloud, Pipe: Daily Scheduled Cron: Automated Drift Detection Pipeline
```

### 3. Branching Strategy & Pipeline Governance
- **Trunk-Based Branching Strategy**: Developers work on short-lived feature branches (`feature/*`, `fix/*`) and integrate frequently into `main`.
- **Branch Policies**: Enforced branch protection on `main` — no direct pushes, no branch deletion, mandatory PR review (min 2 reviewers), and required status checks.
- **Modular Pipeline Templates**: Built reusable YAML templates for:
  - `Validate & Test`
  - `Build & Package`
  - `Deployment & Apply`
  - `Rollback on Failure`
- **Parallel Jobs**: Optimized execution speed using parallel pipeline stages for multi-environment checks.
- **Custom Data & Middleware Setup**: Provisioned VM software, packages, and middleware configurations via custom data scripts and Cloud-init.

---

## 🐳 Containerization & Kubernetes (AKS)

- **Docker Containerization**:
  - Authored clean, optimized multi-stage Dockerfiles.
  - Used lightweight base images (Alpine/Distroless) with non-root security standards.
  - Managed container images securely inside Azure Container Registry (ACR).
- **Azure Kubernetes Service (AKS)**:
  - Deployed and maintained AKS clusters with separate system and user node pools using Virtual Machine Scale Sets (VMSS).
  - Configured Azure CNI networking and pod security.
  - Set up Ingress Controllers (NGINX / AGIC) and automated SSL/TLS certificate renewals.
  - Integrated Azure Key Vault Secrets Store CSI Driver to securely mount secrets as volumes in pods.
  - Container image vulnerability scanning integrated into CI/CD pipelines with Trivy.

---

## 🚀 100+ Enterprise Application Cloud Migration

Hands-on contribution to migrating **100+ multi-tier workloads** from On-Premises Datacenters to Azure across **Dev, UAT, and Production** environments.

```mermaid
flowchart LR
    subgraph Phase1["1. Discovery & Assessment"]
        A1["Server & Application Inventory<br/>(Azure Migrate)"]
        A2["CIDR Assessment &<br/>Dependency Mapping"]
        A3["6R Strategy<br/>(Rehost, Replatform, Refactor)"]
    end

    subgraph Phase2["2. Landing Zone Readiness"]
        B1["Sub Provisioning<br/>(Dev / UAT / Prod)"]
        B2["Hub-Spoke Network &<br/>Firewall Rules"]
        B3["Entra ID & RBAC Setup"]
    end

    subgraph Phase3["3. Migration & Cutover"]
        C1["Data Replication Sync<br/>(ASR / DMS)"]
        C2["Pre-Cutover Checklist<br/>Validation"]
        C3["Cutover Window &<br/>DNS Switch"]
    end

    subgraph Phase4["4. Post-Cutover & Hypercare"]
        D1["Post-Cutover Checklist<br/>& Verification"]
        D2["Monitoring & Alerts<br/>Setup (Azure Monitor)"]
        D3["Hypercare Support &<br/>SOP Documentation"]
    end

    Phase1 --> Phase2 --> Phase3 --> Phase4
```

### Migration Checklists & Execution Governance
| Migration Phase | Action Items & Checklist | Verification Criteria |
| :--- | :--- | :--- |
| **Pre-Migration Checklist** | • Inventory discovery and dependency mapping via Azure Migrate.<br/>• Port readiness and network bandwidth check between On-Prem and Azure.<br/>• Target landing zone readiness (resource groups, subnets, Key Vaults).<br/>• Mock cutover execution in dedicated UAT subscriptions. | All dependencies identified, staging environment validated. |
| **During-Migration Checklist** | • Final delta data sync via Azure Site Recovery / Database Migration Service.<br/>• Graceful shutdown of on-premises application services.<br/>• Database cutover and data consistency validation.<br/>• DNS switchover to Azure public / private endpoints. | Data integrity verified, RPO within agreed window. |
| **Post-Migration Checklist** | • Application smoke testing and end-to-end functionality checks.<br/>• Backup policy enablement (Azure Backup / ASR protection).<br/>• Monitoring agents and Log Analytics data collection validation.<br/>• Sign-off from application owners. | Application healthy, zero critical errors in logs. |
| **Hypercare & Operations** | • 2-4 weeks post-cutover stabilization and issue resolution.<br/>• Performance tuning and resource rightsizing.<br/>• Knowledge Transfer (KT) and Standard Operating Procedures (SOPs) delivery. | Stable workload, smooth transition to BAU operations. |

---

## 🛡️ 4-Tier Security & Governance

```mermaid
graph TD
    subgraph SecurityDefense["4-Tier Defense-in-Depth"]
        Tier1["🔑 1. Identity Level: Microsoft Entra ID | User & Group Management | RBAC | Least Privilege"]
        Tier2["🌐 2. Networking Level: Hub-Spoke | Azure Firewall | UDR Route Tables | NSG/ASG | Private Endpoints"]
        Tier3["📜 3. Governance Level: Azure Policy & Initiatives | Policy Exemptions with Justification"]
        Tier4["💻 4. Compute Level: Hardened OS Images | Defender for Cloud | Disk Encryption | Auto Patching"]
    end
```

- **Identity Level**: Microsoft Entra ID administration, RBAC group assignment, access reviews, and enforcing least privilege access.
- **Networking Level**: Zero public ingress to backend tiers; perimeter security through Azure Firewall, Network Security Groups (NSGs), and forced tunneling via UDRs.
- **Governance Level**: Continuous compliance enforcement with Azure Policy initiatives (e.g. tagging, location restrictions, encryption); structured exemption process with documented justification.
- **Compute Level**: Virtual Machine Scale Sets (VMSS), disk encryption at rest with customer-managed keys (CMK), Defender for Cloud security recommendations, and automated OS patching.

---

## 💰 FinOps & Cloud Cost Optimization

Implemented cost-conscious engineering practices to avoid cloud waste and maintain optimized budgets:

```mermaid
flowchart TD
    FinOps["💡 FinOps Cost Optimization Practices"]
    
    FinOps --> Waste["🗑️ Waste Cleanup"]
    FinOps --> Sizing["📐 Compute Rightsizing"]
    FinOps --> Commit["💳 Reservations & Lifecycle"]
    FinOps --> Telemetry["📊 Telemetry Tuning"]

    Waste --> W1["Identify and delete unattached managed disks"]
    Waste --> W2["Release orphaned public IPs and idle NICs"]
    Waste --> W3["Clean up obsolete snapshots and test resources"]

    Sizing --> S1["Downsize oversized compute based on CPU/RAM metrics"]
    Sizing --> S2["Automated Start/Stop runbooks for Dev & UAT VMs"]
    Sizing --> S3["Use VMSS autoscaling to match active traffic demand"]

    Commit --> C1["Leverage 1-Year / 3-Year Azure Reserved Instances (RI)"]
    Commit --> C2["Storage lifecycle: Hot ➔ Cool ➔ Cold ➔ Archive"]

    Telemetry --> T1["Tune Log Analytics ingestion and filter verbose logs"]
    Telemetry --> T2["Adjust backup retention periods to match compliance requirements"]
    Telemetry --> T3["Enforce cost allocation tags via Azure Policy"]
```

---

## 🔄 High Availability (HA) & Disaster Recovery (BCDR)

- **Storage Redundancy**:
  - **LRS (Locally Redundant)**: Cost-effective storage for non-critical Dev workloads.
  - **ZRS (Zone-Redundant)**: Replicated across availability zones for high-availability production data.
  - **GRS (Geo-Redundant)**: Replicated to secondary paired regions for disaster recovery and compliance backups.
- **Compute High Availability**:
  - Virtual Machine Scale Sets (VMSS) deployed across multiple Availability Zones with auto-healing and scaling rules.
- **Disaster Recovery Planning**:
  - Replicating workloads to secondary regions utilizing **Azure Site Recovery (ASR)**.
  - Adhering to target **Recovery Time Objectives (RTO)** and **Recovery Point Objectives (RPO)** validated through periodic failover drills.

---

## 📈 Monitoring & Observability

- **Azure Monitor & Log Analytics**: Centralized Log Analytics Workspaces (LAW) collecting diagnostic logs, performance counters, and platform metrics.
- **Application Insights**: Tracking application health, request rates, failure rates, and distributed tracing.
- **KQL Queries & Dashboards**: Writing custom Kusto Query Language (KQL) queries to build operational dashboards for infrastructure visibility.
- **Metric Alerts & Action Groups**: Configuring automated alerts for high CPU, disk space thresholds, network latency, and routing notifications to email and webhooks.

---

## 🤝 Project Delivery, Collaboration & Operational Governance

Working collaboratively with cross-functional development, QA, and operations teams:

- **Sprint Participation & Task Ownership**: Active participation in Scrum/Agile ceremonies, user story estimation, technical task execution, and sprint delivery.
- **RFP/RFI & Evaluation Support**: Supported technical evaluation matrices for assessing tooling capabilities, cloud architecture requirements, and operational readiness.
- **SOW & Acceptance Alignment**: Delivered infrastructure milestones according to Statement of Work (SOW) guidelines, acceptance criteria, and technical specifications.
- **Escalation Support**: Designed and followed structured escalation matrices with clear SLA guidelines for incident troubleshooting and resolution.
- **SOP Documentation & KT Transitions**: Authored detailed Standard Operating Procedures (SOPs), operational runbooks, and conducted Knowledge Transfer (KT) sessions for engineering teams.

---

## 🛠️ Technical Skills Ecosystem

<div align="center">

| Domain | Technologies & Tools |
| :--- | :--- |
| **Cloud Platforms** | <img src="https://img.shields.io/badge/Microsoft%20Azure-0089D6?style=flat-square&logo=microsoftazure&logoColor=white" /> <img src="https://img.shields.io/badge/Azure%20CAF-0078D7?style=flat-square" /> <img src="https://img.shields.io/badge/Multi--Subscription-005A9C?style=flat-square" /> |
| **CI/CD & DevSecOps** | <img src="https://img.shields.io/badge/Azure%20Pipelines-0078D7?style=flat-square&logo=azuredevops&logoColor=white" /> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" /> <img src="https://img.shields.io/badge/Trivy-005A9C?style=flat-square" /> <img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white" /> |
| **Infrastructure as Code** | <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" /> <img src="https://img.shields.io/badge/Bicep-0078D7?style=flat-square&logo=azuredevops&logoColor=white" /> <img src="https://img.shields.io/badge/Infracost-00D084?style=flat-square" /> <img src="https://img.shields.io/badge/TFLint-555555?style=flat-square" /> |
| **Containers & Orchestration** | <img src="https://img.shields.io/badge/Kubernetes%20(AKS)-326CE5?style=flat-square&logo=kubernetes&logoColor=white" /> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" /> <img src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white" /> <img src="https://img.shields.io/badge/ACR-0078D7?style=flat-square" /> |
| **Networking & Perimeter** | <img src="https://img.shields.io/badge/Hub%20%26%20Spoke-0078D7?style=flat-square" /> <img src="https://img.shields.io/badge/Azure%20Firewall-FF6F00?style=flat-square" /> <img src="https://img.shields.io/badge/UDR%20Routing-555555?style=flat-square" /> <img src="https://img.shields.io/badge/Private%20Endpoints-2EA44F?style=flat-square" /> <img src="https://img.shields.io/badge/VPN%20Gateway-0089D6?style=flat-square" /> |
| **Security & Identity** | <img src="https://img.shields.io/badge/Microsoft%20Entra%20ID-0078D4?style=flat-square" /> <img src="https://img.shields.io/badge/Azure%20Policy-0078D7?style=flat-square" /> <img src="https://img.shields.io/badge/Defender%20for%20Cloud-002B49?style=flat-square" /> <img src="https://img.shields.io/badge/Azure%20Key%20Vault-FFB900?style=flat-square" /> |
| **Monitoring & BCDR** | <img src="https://img.shields.io/badge/Azure%20Monitor-0089D6?style=flat-square" /> <img src="https://img.shields.io/badge/Log%20Analytics%20(KQL)-005A9C?style=flat-square" /> <img src="https://img.shields.io/badge/Application%20Insights-68217A?style=flat-square" /> <img src="https://img.shields.io/badge/ASR%20%26%20Backup-2EA44F?style=flat-square" /> |
| **Scripting & Automation** | <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" /> <img src="https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white" /> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/YAML-CB171E?style=flat-square&logo=yaml&logoColor=white" /> |
| **Practices & Collaboration** | <img src="https://img.shields.io/badge/FinOps-00C49F?style=flat-square" /> <img src="https://img.shields.io/badge/Agile%20%2F%20Scrum-0078D7?style=flat-square" /> <img src="https://img.shields.io/badge/SOPs%20%26%20Runbooks-555555?style=flat-square" /> <img src="https://img.shields.io/badge/KT%20Transitions-1B263B?style=flat-square" /> |

</div>

---

## 📊 GitHub Activity & Insights

<div align="center">

<table border="0">
  <tr>
    <td align="center">
      <img src="https://github-readme-stats.vercel.app/api?username=simikamble&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1b2a&title_color=0078d4&icon_color=0089D6&text_color=e0e1dd" alt="Simran's GitHub Stats" />
    </td>
    <td align="center">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=simikamble&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1b2a&title_color=0078d4&text_color=e0e1dd" alt="Top Languages" />
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=simikamble&theme=tokyonight&hide_border=true&background=0d1b2a&stroke=0078d4&ring=0089D6&fire=0078d4&currStreakLabel=0089D6" alt="GitHub Streak" />
    </td>
  </tr>
</table>

</div>

---

## 📬 Let's Connect & Collaborate!

I am always interested in discussing **DevOps practices**, **Azure Cloud Infrastructure**, **Terraform Automation**, **CI/CD Pipelines**, and **Kubernetes**.

<div align="center">

<a href="https://linkedin.com/in/simran-kamble">
  <img src="https://img.shields.io/badge/LinkedIn-Connect%20with%20Simran-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Profile" />
</a>
&nbsp;
<a href="mailto:simrankamble@example.com">
  <img src="https://img.shields.io/badge/Email-Drop%20a%20Message-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email Direct" />
</a>
&nbsp;
<a href="https://github.com/simikamble">
  <img src="https://img.shields.io/badge/GitHub-Explore%20Repositories-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Profile" />
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0078d4,70:1b263b,100:0d1b2a&height=120&section=footer" width="100%" alt="Footer" />

<sub>DevOps Engineer (3+ Years) • Azure Cloud & Automation Specialist • © Simran Kamble</sub>

</div>
