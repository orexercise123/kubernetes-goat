---
sidebar_position: 2
title: ☸️ KIND - Windows
slug: kubernetes-goat-on-kind-windows
---

# ☸️ KiND: Windows - Kubernetes IN Docker: Windows 

[kind](https://sigs.k8s.io/kind) is a tool for running local Kubernetes clusters using Docker container "nodes". kind was primarily designed for testing Kubernetes itself, but may be used for local development or CI.

### Prerequisites

* Install Docker Desktop on Windows, [refer to the docs for installation](https://docs.docker.com/desktop/setup/install/windows-install/)
> ⚠️ Because of license requirements, ensure you can install Docker Desktop on Windows.

* You have `kind` installed and setup locally in your system, [refer to the docs for installation](https://kind.sigs.k8s.io/)
* Ensure you have cluster-admin access to the Kubernetes cluster.
  * Also you have installed the `kubectl` and in the path, [refer to the docs for installation](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
  * Verify by running `kubectl version`
* Ensure you have the `helm` package manager installed and the path, [refer to the docs for installation](https://helm.sh/docs/intro/install)
  * Verify by running `helm version`

### Setup

* First, clone the Kubernetes Goat repository locally by running the following command

```bash
git clone https://github.com/madhuakula/kubernetes-goat.git
```

* Navigate to the folder for setup and installation of the Kubernetes Goat using KiND

```bash
cd kubernetes-goat/platforms/kind-setup
```

* Run the following command to set up the KIND cluster

```bash
setup-kind-cluster-and-goat.ps1
```

* Now we have the Kubernetes Goat setup up and running, refer to [Getting Started for next steps](../getting-started.md)
