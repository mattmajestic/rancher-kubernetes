# 🐮 Rancher Docker Compose 🐮

This is a Docker Compose file for running a [Rancher](https://rancher.com/) server. Rancher is an open-source platform that enables organizations to run and manage Docker and Kubernetes in production. It includes a full Kubernetes distribution, but adds additional features such as multi-tenancy, community catalog, and more. This Docker Compose file uses version 3.9.

## 🚀 Services 🚀

The compose file defines a single service: `rancher`.

### 🐮 Rancher 🐮

The Rancher service uses the latest Rancher image from Docker Hub. It runs in privileged mode and exposes ports 80 and 443. It also mounts a volume `rancher_home` at `/var/lib/rancher` in the container.

## 💾 Volumes 💾

The compose file defines a single volume: `rancher_home`. This volume is used by the Rancher service.

## 🏃‍♂️ Running the Services 🏃‍♂️

` docker-compose up`

Run 

## Kubernetes Shell Commands

To add a Helm repository, use the `helm repo add` command. For example, to add the Bitnami repository:

```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install my-nginx bitnami/nginx
```