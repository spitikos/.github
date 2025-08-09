<div align="center">
  <img src="https://raw.githubusercontent.com/spitikos/spitikos/main/assets/icon.svg" alt="spitikos logo" width="150">
  <h1>spitikos</h1>
  <p><i>(σπιτικός) — homemade</i></p>
  <p>A modern, GitOps-driven homelab platform running on a Raspberry Pi.</p>
</div>

---

## 🏡 What is Spitikos?

**Spitikos** is a personal cloud platform built to explore cloud-native technologies in a homelab environment. It leverages a Raspberry Pi 5 to run a complete Kubernetes (k3s) ecosystem, managed entirely through GitOps principles. The entire state of the cluster—from application deployments to infrastructure configuration—is declared in code and synchronized automatically.

This organization houses all the components of the platform, separated into a multi-repo architecture that emphasizes separation of concerns and maintainability.

## ✨ Core Principles

-   **GitOps:** The repositories in this organization are the single source of truth. All changes are made through Git commits, providing an auditable and revertible history.
-   **Automation:** The entire lifecycle, from a code push to a live deployment, is fully automated via GitHub Actions and Argo CD.
-   **Multi-Repo Architecture:** Each component of the platform (application code, Helm charts, core configuration) lives in its own dedicated repository.
-   **Cloud-Native:** The project utilizes modern, cloud-native tools and practices, including Kubernetes, Helm, Prometheus, and Traefik.

##  repositories

The platform is composed of several key repositories:

| Repository                               | Description                                                              |
| :--------------------------------------- | :----------------------------------------------------------------------- |
| 🏛️ [**spitikos**](https://github.com/spitikos/spitikos) | The central repository containing Argo CD manifests, documentation, and reusable CI/CD workflows. |
| 📜 [**charts**](https://github.com/spitikos/charts)     | A collection of all the Helm charts used to deploy applications and platform services. |
| 🏠 [**homepage**](https://github.com/spitikos/homepage)   | The source code for the main web frontend, which includes a dashboard for cluster metrics. |

## 🛠️ Technology Stack

-   **Hardware:** Raspberry Pi 5
-   **Orchestration:** k3s (Kubernetes)
-   **GitOps:** Argo CD
-   **CI/CD:** GitHub Actions
-   **Ingress:** Cloudflare Tunnel & Traefik
-   **Monitoring:** Prometheus & Grafana
-   **Application Packaging:** Helm
