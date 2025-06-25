# Kubernetes Cluster Setup with Ansible

This repository automates the setup of a multi-node Kubernetes cluster using Ansible and Vagrant.

## Project Structure

- `common/` – Shared configuration for all nodes (SELinux, swap, containerd, etc.)
- `master/` – Tasks for initializing the Kubernetes control plane
- `worker/` – Tasks to join worker nodes to the cluster
- `inventory.ini` – Inventory file listing all VMs

## Prerequisites

- Vagrant & VirtualBox
- Git
- Ansible

## Usage

```bash
vagrant up          # Starts and provisions 4 VMs
ansible-playbook -i inventory.ini site.yml
# Kubernetes Cluster Setup with Ansible

This repository automates the setup of a multi-node Kubernetes cluster using Ansible and Vagrant.

## Project Structure

- `common/` – Shared configuration for all nodes (SELinux, swap, containerd, etc.)
- `master/` – Tasks for initializing the Kubernetes control plane
- `worker/` – Tasks to join worker nodes to the cluster
- `inventory.ini` – Inventory file listing all VMs

## Prerequisites

- Vagrant & VirtualBox
- Git
- Ansible

## Usage

```bash
vagrant up          # Starts and provisions 4 VMs
ansible-playbook -i inventory.ini site.yml
# K8s-ansible-cluster
