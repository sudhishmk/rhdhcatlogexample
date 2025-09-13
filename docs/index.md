# 🚀 20-Day Argo CD Mastery Plan

Welcome! This repository contains the practical exercises for a 30-day learning plan designed to take you from an intermediate understanding of Argo CD to a production-ready, expert level.

This plan is structured to require only 15-20 minutes of hands-on learning per day. Each day builds upon the last, culminating in a complete, GitOps-managed project.

---
## ✅ Prerequisites

Before you begin, please ensure you have the following setup:

* **Kubernetes Cluster**: A running cluster is required. This can be a local one like [Minikube](https://minikube.sigs.k8s.io/docs/start/), [k3d](https://k3d.io/), or a cloud-based cluster (GKE, EKS, AKS).
* **Argo CD Installed**: A working installation of Argo CD in your cluster. If you need to install it, you can follow the [official guide](https://argo-cd.readthedocs.io/en/stable/getting_started/).
* **CLI Tools**: `kubectl` and `helm` installed and configured to point to your cluster.
* **Git Repository**: A personal public Git repository (on GitHub, GitLab, etc.) that you can push your work to.

---
## 🗓️ The Daily Structure

Each day's lesson is broken down into five distinct sections to maximize learning:

* **🧠 Concept of the Day:** A brief, direct explanation of a single, focused technical concept.
* **💼 Real-World Use Case:** A practical example of how this concept is used in a professional DevOps/SRE role.
* **💻 Code/Config Example:** A concise, working code snippet or configuration file that demonstrates the concept.
* **🛠️ Daily Task:** A hands-on exercise to apply the day's concept. This is the most important part!
* **🤔 Daily Self-Assessment:** A single question to test your understanding.

---
## 🗺️ Weekly Breakdown

The 30-day plan is divided into four thematic weeks.

### ### Week 1: The Foundation
This week focuses on the fundamentals. You'll set up your first application and learn how to manage it using different tools and strategies.
* **Topics**: The `Application` CRD, automated sync policies, managing apps with **Helm** and **Kustomize**, controlling deployment order with **Sync Waves**, and running imperative tasks with **Sync Hooks**.

### ### Week 2: Scaling & Automation
This week is about managing applications at scale and implementing more advanced deployment patterns.
* **Topics**: Automating application creation with **ApplicationSets** (using Git, Cluster, and Matrix generators), progressive delivery with **Argo Rollouts**, advanced diffing, and custom resource health checks.

### ### Week 3: Security & Enterprise Features
This week, we'll harden the setup and integrate enterprise-grade features for security and observability.
* **Topics**: Multi-tenancy with **Projects** and RBAC, SSO integration, comprehensive **Secret Management** (Vault, Sealed Secrets, External Secrets), and setting up **Notifications** for Slack.

### ### Week 4: Operations & Advanced Topics
The final week dives into day-2 operations, performance tuning, and the most advanced architectural patterns.
* **Topics**: Automating image updates with **Argo CD Image Updater**, custom plugins, advanced CLI usage, performance tuning, disaster recovery, and mastering the **App of Apps** pattern.

---
## 📂 Recommended Repository Structure

As you progress through the daily tasks, your repository will grow. It's recommended to follow a structure similar to this for clarity:
```
argocd-learning/
├── app-of-apps/
│   └── root-app.yaml         # For the final App of Apps pattern
├── echo-chamber/
│   ├── base/                 # Kustomize base resources
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   ├── job.yaml
│   │   └── kustomization.yaml
│   └── overlays/             # Kustomize overlays for different environments
│       ├── dev/
│       │   ├── patch.yaml
│       │   └── kustomization.yaml
│       └── staging/
│           ├── patch.yaml
│           └── kustomization.yaml
└── README.md                 # This file
```
---
## ✨ Final Goal

By the end of this 30-day plan, you will have built a complete GitOps workflow for a sample application, managing multiple environments, handling secrets securely, and automating deployments from start to finish.

Happy GitOps-ing!
