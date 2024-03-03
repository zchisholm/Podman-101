# Podman-101
Repo for documentation of getting started with Podman
> Author: Zedd Chisholm
> 
# Getting Started with Podman

## Introduction
- Brief overview of Podman and its unique features compared to traditional container tools.
- Explanation of Podman's daemonless architecture and support for rootless containers.

## Prerequisites
- General prerequisites for installing Podman across all supported operating systems.
- Note on the necessity of virtualization support for Windows and Mac users.

## Installation Guide

### Windows

#### Installing Podman on Windows
- Instructions on using Windows Subsystem for Linux (WSL) 2 to run Podman.
- Steps to enable WSL 2 and install a Linux distribution from the Microsoft Store.
- Detailed guide for installing Podman within the chosen Linux distribution.

#### Configuring Podman on Windows
- Tips for setting up the Podman environment, including WSL 2 configurations and Linux distribution management.
- Optional configurations for enhancing networking and storage with Podman on Windows.

### Mac

#### Installing Podman on Mac
- Information on Podman Desktop for Mac and alternative installation methods, such as using Podman machine.
- Instructions for downloading and installing Podman Desktop or using Homebrew for installation.

#### Configuring Podman on Mac
- Steps for initial setup with Podman Desktop or initializing a Podman machine.
- Integration tips for terminal and shell environments on Mac.

### Linux

#### Installing Podman on Linux
- Installation instructions for popular Linux distributions like Ubuntu, Fedora, and CentOS, including commands for adding repositories and installing Podman.

#### Configuring Podman on Linux
- Basic configuration steps post-installation, emphasizing Podman's ease of setup due to its daemonless nature.

## Getting Started with Podman

### Running Your First Container
- Commands to run a container with Podman, showcasing the similarity and differences with Docker commands.
- Discussion on the advantages of running containers rootlessly.

### Building and Managing Containers
- Guide on creating containers from Dockerfiles and basic container lifecycle management (start, stop, remove, logs).

### Networking with Podman
- Introduction to networking features in Podman, including container linking and port exposure.

### Podman Compose
- Overview of using Podman Compose for managing multi-container setups.
- Example of converting a `docker-compose.yml` file for Podman Compose.

## Advanced Topics

### Podman and Kubernetes
- How to generate Kubernetes YAML from Podman containers and apply them.
- Example commands for Kubernetes integration.

### Podman in CI/CD Pipelines
- Discussion on incorporating Podman into CI/CD workflows.
- Comparison of Podman and Docker in the context of CI/CD.

## Troubleshooting Common Issues
- Advice for resolving frequent installation and operational problems with Podman.

## Conclusion
- Summary of Podman's benefits and encouragement for further exploration.
- Links to Podman's official documentation and community forums for additional support.

## Appendices

### A. Reference Links
- Official Podman documentation, GitHub repository, and community forums.

### B. Podman vs. Docker CLI Commands
- Table comparing Podman and Docker command-line interfaces to assist users transitioning from Docker.
