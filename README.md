# Hello. I'm Sai Kalyan. 👋

### DevOps Engineer
### based in Brookline, MA

> I architect cloud-native infrastructure end to end, from provisioning through production-grade security.
> Passionate about Kubernetes, GitOps, and multi-cloud architectures.

<br>

| 📧 Email | saikalyanx1@gmail.com |
|----------|---------------------------|
| 🔗 LinkedIn | [linkedin.com/in/sai-kalyan-burra](https://linkedin.com/in/sai-kalyan-burra) |
| 🌐 Portfolio | [saikalyanbportfolio.vercel.app](https://saikalyanbportfolio.vercel.app/) |
| ✍️ Blog | [medium.com/@saikalyan.burra](https://medium.com/@saikalyan.burra) |

<br>

## About Me

Built and scaled a 50+ microservice platform on AWS EKS using Terraform, Kubernetes, and GitOps practices, cutting environment provisioning to 25 minutes and reducing CI/CD pipeline runtime by 80%. Complemented this with independent freelance work administering core AWS services for small business clients, and hold multi-cloud credentials spanning GCP and OCI.

<table>
<tr>
<td width="50%" valign="top">

### 🎓 Education
**MS in Software Engineering Systems**
Northeastern University
*Sep 2024 – Apr 2026*

Coursework: Network Structures & Cloud Computing, Linux for Networking, Operating Systems

</td>
<td width="50%" valign="top">

### 💼 Experience
**Linux System Admin Volunteer** — American Technology Initiative *(Jun 2026 – Present)*
Production-ready 2-node Kubernetes cluster for a nonprofit, from bare hosts to orchestration foundation

**Freelance Web & Cloud Systems Consultant** — Independent *(Nov 2023 – Feb 2024)*
Linux EC2 administration, S3-based static hosting, serverless image processing pipelines

**Software Engineer Intern** — Builtin Tech *(Feb 2023 – Jul 2023)*
5-person team lead · Firebase backend · FinOps dashboards · S3 security hardening

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛠️ Core Skills
- **Cloud & IaC:** AWS (EC2, VPC, S3, RDS, IAM, EKS, ECR, ECS/Fargate, Lambda, CloudWatch, Route 53), GCP (GKE, Cloud SQL), Terraform, CloudFormation
- **Containers & GitOps:** Docker, Kubernetes (EKS/GKE), Helm, Istio, GitHub Actions, ArgoCD, GitLab
- **Observability & Security:** Prometheus, Grafana, Loki, Tempo, HashiCorp Vault, OPA Gatekeeper, Trivy, IAM Policies
- **Linux & Networking:** Ubuntu 24.04, CentOS, systemd, SSH hardening, UFW, fail2ban, Nginx, TLS/certbot, TCP/IP, DNS, VPC/Subnet Design, mTLS
- **Languages:** Python, Bash/Shell, Java, JavaScript, TypeScript, Go

</td>
<td width="50%" valign="top">

### 📜 Certifications
- ✅ Oracle Cloud Infrastructure (OCI) Associate
- ✅ Google Cloud Digital Leader
- 🔄 AWS Certified Solutions Architect — Associate *(In Progress)*

### 📊 Key Metrics
| Metric | Result |
|--------|--------|
| Microservices scaled | 3 → 50+ |
| Environment provisioning | ~25 min |
| CI pipeline runtime | ~80% reduction |

</td>
</tr>
</table>

<br>

## Featured Projects

### ⚡ ShipForge — Cloud-Native CI/CD & Microservices Platform
> Scaled from 3 to 50+ microservices on AWS EKS with a full GitOps workflow

- Reusable Terraform modules with a `for_each` pattern — environment provisioning cut to ~25 minutes
- GitHub Actions dynamic matrix builds with change detection — ~80% pipeline runtime reduction
- ArgoCD ApplicationSets with Git directory generators — net-new service deploys down to a single directory commit
- Full-stack observability: Prometheus, Grafana, Loki, Tempo, with Kubecost for per-service cost accountability
- Zero-trust security baseline: Kubernetes Network Policies, Istio mTLS, HashiCorp Vault, OPA Gatekeeper

**Tech:** `AWS EKS` `Terraform` `ArgoCD` `Helm` `Docker` `GitHub Actions` `Prometheus` `Grafana` `Istio` `Vault` `OPA Gatekeeper`

---

### 🤖 InfraLens — AI-Powered Terraform Review Pipeline
> GitHub Actions pipeline using the Claude API to review infrastructure diffs on PRs

- Analyzes Terraform diffs on PRs and blocks merges on critical findings via OPA Rego policy gates, validated against ShipForge's production EKS codebase
- Filters low-level noise through tflint and Checkov before AI analysis, then structures Claude's output as JSON so OPA can auto-enforce policy gates and post inline PR feedback

**Tech:** `GitHub Actions` `Claude API` `OPA Rego` `tflint` `Checkov`

---

### 🔧 OpsiMate — Open Source Contributor
> Terraform modules & Helm charts for an open-source alert management platform

- PRs #256 and #257 merged upstream — Helm chosen over raw manifests so contributors could override environment values without touching templates, cutting onboarding from 4+ hours to under 10 minutes
- Established PR-level quality gates: Helm chart linting, Terraform plan validation, automated unit tests

**Tech:** `Terraform` `Helm` `Kubernetes` `AWS EKS` `EC2` `GitHub Actions`

---

### 🖥️ LinuxOps Homelab — Production Server Hardening & Operations
> Hardened Ubuntu 24.04 EC2 server with a full operational runbook

- SSH key-only auth, UFW firewall, fail2ban brute-force protection, and an Nginx reverse proxy with TLS termination and security headers (HSTS, X-Frame-Options)
- Node Exporter deployed as a systemd service exposing CPU, disk, and memory metrics
- Automated disk usage reporting via cron and logrotate, with a full operational runbook covering all procedures

**Tech:** `Ubuntu 24.04` `Nginx` `Let's Encrypt` `UFW` `fail2ban` `Node Exporter` `systemd` `cron` `logrotate`

📂 [Repo](https://github.com/Sai9700128/linux-ops-homelab)

---

### 🔄 Multi-Region Disaster Recovery on AWS
> Active-passive DR across two AWS regions with automated failover

- **RPO:** 5 minutes | **RTO:** 15 minutes
- Route 53 health checks + DNS failover + cross-region replication
- Zero human involvement during simulated regional outages

**Tech:** `Terraform` `AWS (EC2, RDS, S3, Route 53, Lambda, CloudWatch)` `GitHub Actions` `Bash`

📂 [Repo](https://github.com/Sai9700128/Multi-Region-DR)

---

### 🏠 Roomies Radar — Roommate Matching Platform
> Full-stack PWA connecting individuals with compatible roommates

- JWT authentication · Preference-based matching · Domain-Driven Design · PWA

---

### 🖥️ MyOS — Interactive Operating System from Scratch
> A 32-bit x86 kernel built from bare metal, booting into an interactive command shell in QEMU

- Wrote a custom bootloader and kernel in x86 Assembly, running in 32-bit protected mode with direct VGA text-mode display (80x25) output
- Built a keyboard-driven command loop handling PS/2 input, with a working shell supporting `clear`, `help`, `info`, `list`, `hello`, `mem`, and `time` commands
- Implemented low-level system introspection (OS version, mode, display, and input device reporting) entirely from raw hardware interaction, with no OS or libc underneath

**Tech:** `x86 Assembly (NASM)` `QEMU` `Make` `Bare-metal / OS Development`

<br>

---

<p align="center">
  <b>Available for Cloud / DevOps / SRE / Platform Engineer roles · F-1 OPT Authorized · H-1B Sponsorship Required Long-Term · Open to Relocation</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/sai-kalyan-burra">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="mailto:saikalyanx1@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail" />
  </a>
  <a href="https://saikalyanbportfolio.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-Visit-brightgreen?style=for-the-badge&logo=vercel" />
  </a>
</p>
