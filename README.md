# Dockyard

> A modern SwiftUI dashboard and companion application for self-hosted infrastructure.

**Dockyard** is a native Apple application designed to simplify the monitoring of home servers, NAS devices and homelab environments through a clean, unified and mobile-first interface.

The project is currently under development for **iOS**, with planned support for **macOS** in future releases.

---

# Status

🚧 This project is currently under active development.

The current version uses mock JSON data to validate the application's architecture and user interface before integrating with real server APIs.

---

# Overview

Managing a self-hosted server often requires interacting with multiple independent dashboards.

Whether hosting media servers, cloud storage, password managers or Docker containers, users usually need to switch between several web interfaces just to understand the overall health of their infrastructure.

Dockyard centralizes essential system information into a single, intuitive application built with SwiftUI, allowing users to quickly inspect their infrastructure from anywhere.

---

# Problem Statement

The popularity of self-hosting has grown significantly over the last few years.

Users increasingly rely on home servers to host services such as:

- Personal cloud storage
- Media streaming
- Password managers
- Home automation
- Game servers
- File synchronization
- AI workloads
- Network services

Although these solutions provide greater privacy, ownership and flexibility, monitoring them typically requires several disconnected dashboards.

This fragmentation makes it difficult to quickly understand the health and availability of an entire infrastructure.

Dockyard aims to solve this problem by providing a unified monitoring experience.

---

# Objectives

Dockyard aims to:

- Centralize server information into a single application.
- Provide a clean, Apple-native user experience.
- Reduce the time required to inspect infrastructure health.
- Allow quick identification of failures.
- Offer a lightweight companion experience instead of replacing existing management platforms.
- Support future integrations with multiple self-hosted ecosystems.

---

# Target Users

Dockyard is designed for:

- Homelab enthusiasts
- NAS owners
- Home server administrators
- Developers
- Small businesses
- Students learning self-hosting technologies

---

# Current MVP

The first version focuses exclusively on infrastructure monitoring.

Current features include:

- CPU usage
- Memory usage
- Storage utilization
- CPU temperature
- Service availability
- Overall server status

The MVP intentionally relies on local mock JSON data while the application's architecture is validated.

---

# Roadmap

## Infrastructure Monitoring

- CPU usage
- Memory usage
- Swap usage
- Storage usage
- SMART drive health
- Drive temperatures
- CPU temperature
- Fan speed
- Network throughput
- System load
- Uptime
- UPS / Battery status

---

## Containers

- Docker container monitoring
- Container health
- Start / Stop containers
- Restart containers
- Container logs

---

## Storage

- RAID status
- Storage pools
- Available capacity
- SMART information
- Disk failure detection

---

## Alerts & Notifications

- High CPU usage
- High memory usage
- Disk almost full
- High temperature
- Offline services
- Failed backups
- SMART warnings

---

## Backups

- Last backup
- Backup history
- Backup failures
- Scheduled backups

---

## Networking

- Local IP
- Public IP
- VPN status
- Tailscale status
- WireGuard status

---

## Supported Services (Planned)

- Jellyfin
- Immich
- Nextcloud
- Vaultwarden
- Home Assistant
- Pi-hole
- AdGuard Home
- Syncthing
- Grafana
- Prometheus
- Uptime Kuma

---

## Planned Integrations

- Docker Engine API
- TrueNAS API
- Proxmox API
- CasaOS
- OpenMediaVault
- Portainer
- Home Assistant
- Tailscale

---

# Long-term Vision

Dockyard is not intended to replace existing server management platforms.

Instead, it aims to become a lightweight companion application that provides users with a fast overview of the health, availability and status of their self-hosted infrastructure from anywhere.

---

# Tech Stack

- Swift
- SwiftUI
- MVVM Architecture
- Codable
- JSON
- URLSession *(planned)*
- REST APIs *(planned)*

---

# Architecture

```
SwiftUI Views
        │
        ▼
 ViewModels
        │
        ▼
   Services
        │
        ▼
 REST APIs
        │
        ▼
Home Server
```

---

# Why Dockyard?

As the self-hosting community continues to grow, monitoring infrastructure often requires interacting with multiple independent dashboards.

Dockyard explores how a native Apple experience can reduce this complexity by presenting essential information through a single, cohesive and mobile-first interface.

The goal is not to replace existing tools, but to complement them by making infrastructure monitoring faster, simpler and more accessible.

---

# Design Philosophy

Dockyard follows Apple's Human Interface Guidelines and embraces a mobile-first approach.

The application prioritizes:

- Simplicity
- Clarity
- Accessibility
- Fast information retrieval
- Native Apple design patterns

Rather than exposing every available server configuration, Dockyard focuses on presenting the most relevant information at a glance, enabling users to understand the health of their infrastructure within seconds.

---

# Disclaimer

Dockyard is an independent open-source project and is not affiliated with or endorsed by Apple Inc., Docker Inc., TrueNAS or any of the third-party platforms referenced in this repository.
