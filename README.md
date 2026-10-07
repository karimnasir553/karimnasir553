# Abdul Karim Nasir Siddiqui
 
**Platform and DevOps engineer in Nürnberg, Germany.** Kubernetes, Terraform, Ansible, Python — and I operate what I build, which is the part that changes how carefully you build it.
 
Currently working on cloud platform and infrastructure at WSAudiology, and finishing an M.Sc. at FAU Erlangen-Nürnberg focused on AI systems and data-driven methods. My first degree is electrical engineering, so I came to software from the hardware side.
 
**Available from November 2026.**
 
---
 
### What I actually do
 
Infrastructure as code rather than consoles — reusable Terraform modules, role-based Ansible across a bare-metal hypervisor fleet, every change through pull request and review. Multi-stage CI/CD with coverage gates, linting and type checking enforced in the pipeline. Kubernetes in production on AWS and Azure, and a self-managed K3s cluster of my own. Prometheus, Grafana and Loki for the parts that have to be visible at 3am.
 
I also own two stages of a nightly production data pipeline end to end — a Python service with idempotent PostgreSQL ingestion and a TypeScript frontend, built and operated by me rather than handed over.
 
---
 
### How I think about building things
 
These aren't slogans — each one came from something that went wrong.
 
**Idempotent by construction.** A rerun after a partial failure should be *always* safe, not usually safe. Get that property in before you need it and recovery becomes "run it again" instead of working out which of twelve steps completed.
 
**Fail closed, and refuse ambiguous input.** For anything destructive, stopping is better than resolving to the most likely answer.
 
**Enforcement beats documentation.** A gate in the pipeline holds. A convention in a style guide decays quietly.
 
**Declared inventory, not derived.** A collector that builds its target list by traversal is permanently silent about whatever it can't reach — and you can't alert on the absence of something nobody declared should exist. I learned this the hard way, from 27 machines that had never been monitored at all.
 
**The simpler design, argued with measurements.** I benchmarked two concurrency designs over five trials each and made the case for the less sophisticated one, including being honest that two of the runs were within noise.
 
---
 
### Projects
 
**[linux-k8s-homelab](https://github.com/karimnasir553/linux-k8s-homelab)** — Self-managed Kubernetes from the ground up. Terraform provisions VMs on Proxmox, Ansible applies Linux baselines, K3s on top, ArgoCD for GitOps delivery, Vault for secrets and certificates, Kyverno enforcing policy at admission, with SLOs under an error-budget policy. Built because the way to understand what a managed control plane does for you is to not have one.
 
**[devops-flagship](https://github.com/karimnasir553/devops-flagship)** — An internal developer platform on AWS. EKS with reusable Terraform modules, a Backstage portal whose software templates scaffold new services, GitHub Actions publishing to ECR, ArgoCD delivery, Prometheus and Grafana. The idea being that a platform team shouldn't be a ticket queue — you encode the conventions into the platform instead of dispensing them one request at a time.
 
**[cloud-native-microservices](https://github.com/karimnasir553/cloud-native-microservices)** — Containerised Python microservices with CI/CD and Kubernetes delivery.
 
**[MA_Siddiqui](https://github.com/karimnasir553/MA_Siddiqui)** — M.Sc. thesis work: AI systems and data-driven methods.
 
---
 
### Stack
 
**Languages** — Python, Bash, SQL, TypeScript, C++, YAML, PromQL
 
**Infrastructure** — Terraform, Ansible, Proxmox, Linux (systemd, storage, networking), Windows Server + AD
 
**Containers** — Docker, Kubernetes (EKS, AKS, K3s), Helm, ArgoCD, Kyverno
 
**Cloud** — AWS (EKS, IAM, ECR, VPC), Azure (AKS, DevOps, Key Vault)
 
**CI/CD** — GitHub Actions, Azure DevOps, GitLab, Jenkins
 
**Data & observability** — PostgreSQL, Prometheus, Grafana, Loki, InfluxDB
 
---
 
### On AI tooling
 
A year of daily work with Claude Code — the projects here were built with it, and so is a good deal of my production work.
 
The discipline matters more than the usage: give the agent the context it actually needs, break a change into steps that can be verified independently, and review the output as if a colleague wrote it. I'm the one accountable for architecture, security and what reaches production, and that doesn't transfer to a tool.
 
---
 
### Contact
 
[LinkedIn](https://www.linkedin.com/in/abdul-karim-nasir-siddiqui-5a724022a/) · karimnasir97@gmail.com