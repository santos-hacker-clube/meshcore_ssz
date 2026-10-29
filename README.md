# Baixada Santista MeshCore Network Expansion

[![Network: MeshCore](https://img.shields.io/badge/Network-MeshCore-blue.svg)](https://github.com/meshcore)

An open-source, community-driven project to build and expand an off-grid, decentralized LoRa mesh communication network across the Baixada Santista metropolitan region (São Paulo, Brazil).

---

## 📌 Project Overview

Extreme weather events and climate-related disasters frequently compromise traditional communication infrastructure (power grids, cellular networks, and internet service providers). 

This project aims to enhance community resilience in the Baixada Santista region by deploying a reliable, off-grid MeshCore LoRa network. The system serves a dual purpose:
1. **Daily Social & Community Use:** Facilitating local peer-to-peer communication, community organizing, and decentralized messaging.
2. **Emergency Response & Disaster Relief:** Providing a standalone, resilient communication backbone during severe weather crises, floods, landslides, and infrastructure outages.

---

## 🎯 Objectives & Scope

- **Deploy 5 Strategic Repeaters:** Install solar-powered outdoor repeaters across high-elevation and key coverage points in Baixada Santista to ensure robust inter-city backhaul coverage.
- **Set Up Room Servers (Rooms):** Configure localized, persistent digital spaces for community channels, emergency dispatch, and public information sharing.
- **Deploy Observers & Gateways:** Establish passive telemetry and monitoring nodes (Observers) to analyze RF coverage, signal propagation, and network health.
- **Open Documentation & Hardware Standards:** Provide fully documented, reproducible hardware builds, flashing procedures, and enclosure designs for community adoption.

---

## 🏗 Network Architecture

![Mesh Network Topology](https://magnus919.com/2026/05/how-meshcore-scales-where-other-lora-meshes-hit-walls/meshcore-roles-diagram.png)
---

### Node Roles

- **Repeaters (x5):** Solar-powered, weather-proofed relay nodes placed at strategic elevated locations to interconnect cities across the coastal plain.
- **Rooms (Room Servers):** Local message hubs that allow persistent group communications and structured topic channels without relying on central internet servers.
- **Observers:** Specialized monitoring nodes that log network traffic, packet loss, RSSI/SNR metrics, and coverage topology to help optimize node placement.
- **Clients:** End-user handheld or desktop devices connected via Bluetooth, Serial USB, or Wi-Fi to access the network.

---

## 🛠 Hardware Specifications (Target Specs)

| Component | Target Hardware / Standard |
| :--- | :--- |
| **LoRa Boards** | Heltec WiFi LoRa 32 V3, Seeed Studio XIAO nRF52840, or equivalent ESP32/nRF52 boards |
| **Frequency Band** | 915 MHz (AU915 / US915 - Anatel compliant for Brazil) |
| **Power System (Repeaters)** | 18650 / LiFePO4 batteries + MPPT solar charge controller + 5V/6V Solar Panel |
| **Enclosures** | IP67 weatherproof outdoor enclosures with N-type / SMA antenna pass-throughs |
| **Antennas** | 3 dBi - 6 dBi fiberglass omnidirectional antennas for high-elevation repeaters |

---

## 🗺 Deployment Plan

- [ ] **Phase 1: Site Survey & Propagation Modeling**
  - Radio Mobile / CloudRF simulations for the 5 target repeater sites in Baixada Santista.
  - Identification of host sites (community structures, public facilities, elevated terrain).
- [ ] **Phase 2: Hardware Assembly & Bench Testing**
  - Flashing MeshCore firmware and testing node-to-node telemetry.
  - Solar cycle stress testing for repeaters.
- [ ] **Phase 3: Field Deployment**
  - Installation of the 5 primary repeaters.
  - Setup of initial Room Servers and Observer nodes.
- [ ] **Phase 4: Community Onboarding & Crisis Drills**
  - Public workshops on building/configuring client nodes.
  - Simulation of off-grid emergency coordination scenarios.

---

## ⚙️ Software & Configuration

This project relies on the open-source **MeshCore** ecosystem.

- **Firmware:** [MeshCore Firmware](https://github.com/meshcore)
- **CLI & Management Tools:** `meshcore-cli` for node management, channel configuration, and telemetry extraction via USB/BLE.

---

## 🤝 Contributing & Community

Contributions are welcome! Whether you want to host a repeater, test signal coverage in your neighborhood, or contribute to software tooling:

1. Check open **Issues** for current tasks and site survey needs.
2. Join our local mesh radio discussions (see community links below).
3. Submit Pull Requests for setup guides, 3D printable enclosures, or propagation map data.

---
