# ROCm 6.4.3 + OpenCL 2.x + PyTorch 2.9.0 (Nightly) + Transformers + Docker Setup

[![ROCm](https://img.shields.io/badge/ROCm-6.4.3-ff6b6b?logo=amd)](https://rocm.docs.amd.com)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.9.0.dev%2Brocm6.4-ee4c2c?logo=pytorch)](https://pytorch.org)
[![Docker](https://img.shields.io/badge/Docker-28.4.0-blue?logo=docker)](https://www.docker.com/)
[![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04%20%7C%2024.04-e95420?logo=ubuntu)](https://ubuntu.com)

## 📌 Overview
This repository provides an **automated installation script** for setting up a complete **AMD ROCm 6.4.3** development environment with:
- **ROCm 6.4.3** GPU drivers + OpenCL 2.x SDK  
- **PyTorch 2.9.0 (Nightly)** ROCm build  
- **Transformers 4.56.1** + **Accelerate + Diffusers + Datasets**  
- **Docker environment** with AMD GPU support  
- **Preconfigured GPU test scripts**

The setup is fully **non-interactive** and optimized for both **desktop** and **server** deployments.

---

## 🖥️ Supported Platforms

| **Component**      | **Supported Versions**                                |
|---------------------|------------------------------------------------------|
| **OS**            | Ubuntu 22.04.x (Jammy Jellyfish), Ubuntu 24.04.x (Noble Numbat) |
| **Kernel**        | 5.15.x (22.04) • 6.8.x (24.04)                        |
| **GPUs**          | AMD CDNA2 • CDNA3 • RDNA3 • **RDNA4**                 |
| **Docker**        | 28.4.0 (stable)                                       |
| **ROCm**          | 6.4.3                                                |
| **PyTorch**       | 2.9.0.dev20250906+rocm6.4                             |
| **Transformers**  | 4.56.1                                               |

> **⚠️ Note**: **Ubuntu 20.04.x (Focal Fossa)** is **not supported**. The last compatible ROCm version for 20.04 is **6.4.0**.

---

## ⚡ Features
- Automated **ROCm GPU drivers + HIP + OpenCL SDK** installation
- **PyTorch ROCm nightly** with GPU acceleration
- Preinstalled **Transformers**, **Accelerate**, **Diffusers**, and **Datasets**
- Integrated **Docker environment** with ROCm GPU passthrough
- **vLLM Docker images** for **RDNA4** & **CDNA3**
- Optimized for **AI workloads**, **LLM inference**, and **model fine-tuning**

---

## 🚀 Installation

### 1️⃣ **Clone the Repository**
```bash
git clone https://github.com/<your-org>/rocm-6.4.3-rdna4-docker-deployment.git
cd rocm-6.4.3-rdna4-docker-deployment
```
### 2️⃣ **Run the Installer
```bash
bash rocm-6.4.3-setup.sh
```

The installation takes ~15 minutes depending on internet speed and hardware performance.

🐋 Docker Integration

The script sets up a Docker environment with GPU passthrough support via ROCm.

Check Docker Installation
docker --version
