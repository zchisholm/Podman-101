# Podman-101
Repo for documentation of getting started with Podman
> Author: Zedd Chisholm
> 
# Getting Started with Podman

## Introduction

[Podman](https://podman.io/) (Pod Manager) is an open-source tool for developing, managing, and running OCI Containers on your Linux System. Containers can either be run as root or in rootless mode. Unlike traditional container engines, such as Docker, Podman operates without a daemon and provides a Docker-compatible command-line interface (CLI). This design enhances security, reduces complexity, and facilitates easier troubleshooting.

### Unique Features Compared to Traditional Container Tools

Podman distinguishes itself from other containerization tools with several key features:

- **Daemonless Architecture**: Podman does not require a running daemon to manage containers. This design reduces potential attack vectors and simplifies the architecture, making Podman an ideal choice for developers and system administrators who prioritize security and minimal overhead.

- **Rootless Containers**: Podman allows users to run containers without root privileges, significantly enhancing security by limiting the potential impact of container vulnerabilities. This feature is particularly beneficial in multi-user environments and for personal development, as it minimizes the risk of system-wide compromises.

- **Compatibility with Docker**: Podman offers a CLI that is compatible with Docker, making it easy for users to transition without changing their workflows. Docker commands can often be replaced with Podman commands simply by substituting `docker` with `podman`.

- **Pods Support**: Inspired by Kubernetes, Podman can manage groups of containers as a single pod, allowing for easier management of multi-container applications.

- **OCI Compliant**: Podman is fully compliant with the Open Container Initiative (OCI) standards, ensuring compatibility with OCI containers and image specifications.

### Daemonless Architecture and Support for Rootless Containers

Podman’s daemonless architecture means that each command is executed in its own process, avoiding the need for a constantly running background service. This approach not only enhances security by reducing the attack surface but also allows for direct control over containers without intermediaries. Moreover, the support for rootless containers enables users to run containers with their user ID, avoiding the need for escalated privileges and further securing the containerized environment.

Podman integrates seamlessly into the container ecosystem, offering features like image management, volume management, network management, and more, while adhering to a secure and user-friendly approach. Whether you are a developer, system administrator, or DevOps engineer, Podman provides a powerful, secure, and flexible tool for container management.

### Docker vs. Podman Feature Comparison

For those who are familiar with Docker, here is a table comparing the features of Docker and Podman.

| Feature                         | Docker | Podman |
|---------------------------------|--------|--------|
| Daemonless Architecture         | X      | ✓      |
| Rootless Containers             | X      | ✓      |
| Compatibility with Docker CLI   | ✓      | ✓      |
| Pods Support                    | X      | ✓      |
| OCI Compliant                   | ✓      | ✓      |

- "✓" indicates that the feature is supported.
- "X" indicates that the feature is not supported.

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
