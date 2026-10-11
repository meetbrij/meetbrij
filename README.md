<h1 align="center">Brijeshh Harish Bolar</h1>

<p align="center">
  <b>Forward Deployed AI Engineer</b><br>
  I design and ship production AI systems: LangGraph agents, RAG, evals and secure cloud delivery on Azure and AWS<br>
  LLMOps · DevSecOps · Ex-AVP, Bank of Singapore
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/brijeshh-harish-bolar/"><img src="https://img.shields.io/badge/LinkedIn-Brijeshh%20Harish%20Bolar-0A66C2?style=flat" alt="LinkedIn"></a>
  <img src="https://img.shields.io/badge/Based%20in-Mumbai-555?style=flat" alt="Based in Mumbai">
  <img src="https://img.shields.io/badge/Open%20to-UAE%20roles-2E7D32?style=flat" alt="Open to UAE roles">
  <img src="https://img.shields.io/badge/AWS-Solutions%20Architect%20Associate-FF9900?style=flat" alt="AWS Certified Solutions Architect – Associate">
</p>

---

### About me

- I turn business problems into production AI systems: I work out the requirements with the people who own the problem, build the solution (agent workflows, retrieval, API integrations, evaluation), deploy it on Azure or AWS, and stay accountable until it works in production.
- Before this I was AVP and Technical Lead at **Bank of Singapore**, leading a 10+ engineer team on the Enterprise Data Management platform, and earlier built wealth-management and digital-commerce platforms at Standard Chartered and Singtel.
- I work the way regulated industries need: every number measured, every decision written down, no secrets in code, and systems that degrade instead of failing.
- In 2024–25 I ran a small consultancy, Vaiteq Solutions, shipping AI-enabled MVPs for startups. Since 2026 I've been building production-grade AI and cloud systems full time; they're below.

---

### Featured project

#### [Azure Market Intelligence Agent](https://github.com/meetbrij/azure-market-intel-agent)

A research agent for public companies. Ask a question and get a structured report in which every claim cites a specific page of an SEC 10-K or a news URL. Built on LangGraph with human approval, crash-safe checkpointing and an eval gate in CI.

| Result | Measured |
|---|---|
| Retrieval lift (hybrid + semantic ranker vs vector) | context precision **0.54 → 0.81**, recall **0.85 → 1.00** |
| Grounding | faithfulness **0.97**, citation validity **100%** |
| Unanswerable questions correctly declined | **100%** |
| Cost per report (priced by Langfuse) | **$0.071** |
| Worker killed mid-report | resumes from its last checkpoint (Compose, kind and Azure) |
| Tests | **188** offline tests, eval gate on every push |

**Stack:** LangGraph · Azure OpenAI · Azure AI Search · FastAPI · arq + Redis · Postgres · MCP · Langfuse · RAGAS · Bicep · Azure Container Apps · Helm · Azure Pipelines · Entra ID · Key Vault

---

### Other projects

| Project | What it is | Result | Stack |
|---|---|---|---|
| [Client Onboarding Case Workflow](https://github.com/meetbrij/client-onboarding-ai-agent) | A LangGraph agent runs a bank onboarding case end to end: extract documents, screen the UN sanctions list, apply risk rules, wait for a compliance officer, create the customer in a core-banking API. Hash-chained audit trail; controls mapped to the CBUAE AI guidance. Live on EKS | Right steps in **12/12** cases, right recommendation in **11/12**, **3/3** sanctions hits caught | LangGraph · Claude · FastAPI · Postgres · rapidfuzz · EKS · GitHub Actions |
| [KYC Document Intelligence on EKS](https://github.com/meetbrij/prod-grade-e2e-devsecops-pipeline) | Claude reads ID and proof-of-address documents into validated fields with confidence scores and sends uncertain fields to a person. On EKS behind a GitHub Actions pipeline with blocking security gates and approval-gated production | Field accuracy **92.0%** (Haiku 4.5), **99.0%** (Sonnet 5) on 18 synthetic documents | Claude · Amazon Bedrock route · FastAPI · MySQL · Terraform · EKS · GitHub Actions + OIDC · Gitleaks · Checkov · Trivy · SonarCloud · Prometheus · Loki · Tempo · Grafana |
| [3-tier AWS infrastructure](https://github.com/meetbrij/3tier-aws-terraform-jenkins-devops-pipeline) | Multi-AZ web, app and data tiers with immutable AMIs and separate Terraform stacks, delivered through Jenkins | Built | Terraform · Packer · Jenkins · EC2 ASG · ALB · RDS · Secrets Manager |

---

### Tech stack

**AI and agents**
<br>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langchain&logoColor=white" alt="LangGraph">
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white" alt="LangChain">
<img src="https://img.shields.io/badge/Azure%20AI%20Foundry-0078D4?style=flat" alt="Azure AI Foundry">
<img src="https://img.shields.io/badge/Azure%20AI%20Search-0078D4?style=flat" alt="Azure AI Search">
<img src="https://img.shields.io/badge/Claude-D97757?style=flat" alt="Claude">
<img src="https://img.shields.io/badge/Amazon%20Bedrock-232F3E?style=flat" alt="Amazon Bedrock">
<img src="https://img.shields.io/badge/RAGAS-6A1B9A?style=flat" alt="RAGAS">
<img src="https://img.shields.io/badge/Langfuse-111111?style=flat" alt="Langfuse">
<img src="https://img.shields.io/badge/MCP-555555?style=flat" alt="MCP">

**Cloud and platform**
<br>
<img src="https://img.shields.io/badge/Azure-0078D4?style=flat" alt="Azure">
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat" alt="AWS">
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white" alt="Kubernetes">
<img src="https://img.shields.io/badge/Helm-0F1689?style=flat&logo=helm&logoColor=white" alt="Helm">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Terraform-844FBA?style=flat&logo=terraform&logoColor=white" alt="Terraform">
<img src="https://img.shields.io/badge/Bicep-0078D4?style=flat" alt="Bicep">
<img src="https://img.shields.io/badge/Packer-02A8EF?style=flat&logo=packer&logoColor=white" alt="Packer">

**CI/CD and security**
<br>
<img src="https://img.shields.io/badge/Azure%20Pipelines-0078D4?style=flat" alt="Azure Pipelines">
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white" alt="GitHub Actions">
<img src="https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white" alt="Jenkins">
<img src="https://img.shields.io/badge/Trivy-1904DA?style=flat" alt="Trivy">
<img src="https://img.shields.io/badge/Checkov-5B2A86?style=flat" alt="Checkov">
<img src="https://img.shields.io/badge/Gitleaks-555555?style=flat" alt="Gitleaks">
<img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=flat&logo=sonarqube&logoColor=white" alt="SonarQube">

**Engineering**
<br>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white" alt="MySQL">
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" alt="Redis">
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white" alt="Kafka">
<img src="https://img.shields.io/badge/Java%20Spring-6DB33F?style=flat&logo=spring&logoColor=white" alt="Java Spring">

**Observability**
<br>
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white" alt="Prometheus">
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white" alt="Grafana">
<img src="https://img.shields.io/badge/Loki-F46800?style=flat" alt="Loki">
<img src="https://img.shields.io/badge/Tempo-F46800?style=flat" alt="Tempo">
<img src="https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat&logo=opentelemetry&logoColor=white" alt="OpenTelemetry">

---

### Certifications

<p>
  <a href="https://www.credly.com/badges/0d7073a3-3cc1-42e0-a0f7-ff419c2564c5" title="AWS Certified Solutions Architect – Associate (verify on Credly)">
    <img src="https://images.credly.com/images/0e284c3f-5164-4b21-8660-0d84737941bc/image.png" width="110" alt="AWS Certified Solutions Architect – Associate">
  </a>
  &nbsp;
  <a href="https://www.credly.com/badges/25165ca6-f250-42b1-9f37-fce8b9415b54" title="Professional Scrum Master I (verify on Credly)">
    <img src="https://images.credly.com/images/a2790314-008a-4c3d-9553-f5e84eb359ba/image.png" width="110" alt="Professional Scrum Master I">
  </a>
</p>

- **AWS Certified Solutions Architect – Associate** · Amazon Web Services · 2026 · [verify](https://www.credly.com/badges/0d7073a3-3cc1-42e0-a0f7-ff419c2564c5)
- **Professional Scrum Master I (PSM I)** · Scrum.org · 2021 · [verify](https://www.credly.com/badges/25165ca6-f250-42b1-9f37-fce8b9415b54)

<sub>All badges: <a href="https://www.credly.com/users/brijesh-bolar/badges">credly.com/users/brijesh-bolar</a></sub>

---

### How I build

- **Measured, not estimated.** Retrieval changes ship with before/after numbers from a golden set.
- **Degrade, don't fail.** An outage in one source is recorded as a data gap; the run still completes.
- **Keyless by default.** Managed identities and workload identity federation, secrets in a vault, none in code or pipelines.
- **The model advises; rules and people decide.** Risk scores, sanctions matches and approvals stay in deterministic code or with a human, and every step is audited.
- **Decisions on record.** Architecture decision records for anything that would be hard to reverse.

---

<p align="center">
  <a href="https://www.linkedin.com/in/brijeshh-harish-bolar/">LinkedIn</a> · bolar.brijesh@gmail.com
</p>
