# OCTACORE TECHNOLOGIES

> Building resilient communication systems for the moments the network goes down.

**OctaCore Technologies** is an eight-person software engineering team building hardware and software that keeps people connected when conventional infrastructure fails. We work across the full stack of a connected system — embedded firmware, radio networking, backend services, web consoles, and mobile clients — and ship them as one integrated product rather than four disconnected parts.

---

## Stack

**Core**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)

**Web App**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)

**Mobile App**

![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

**Firmware & Comms**

![ESP32](https://img.shields.io/badge/ESP32--S3-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![ESP-IDF](https://img.shields.io/badge/ESP--IDF-000000?style=for-the-badge&logo=espressif&logoColor=E7352C)
![PlatformIO](https://img.shields.io/badge/PlatformIO-F5822A?style=for-the-badge&logo=platformio&logoColor=white)
![Meshtastic](https://img.shields.io/badge/Meshtastic-67EA94?style=for-the-badge&logo=meshtastic&logoColor=black)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)

**Tooling**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=for-the-badge&logo=obsidian&logoColor=white)

---

## About OctaCore Technologies

*OctaCore* is the eight of us — eight cores on one process, each front running in parallel toward a single build.

Our mission is to design systems that stay useful under the worst conditions we can anticipate: no cell towers, no internet backhaul, no reliable power, and operators who need the thing to work on the first try in the dark. That constraint shapes everything from our hardware choices to our UI defaults. We would rather ship something modest that survives the field than something impressive that only works on a bench.

---

## Areas of Focus

- **Disaster-Response Communications** — Systems that restore coordination capability in signal-dead areas after a disaster.
- **LoRa Mesh Networking** — Long-range, low-power multi-hop radio links between field-deployed relay nodes.
- **Embedded Systems & Firmware** — ESP32-class hardware, power budgeting, and enclosure-level field durability.
- **Full-Stack Web Development** — Coordination consoles with live mapping, node health, and placement guidance.
- **Offline-First Mobile** — Field apps that assume no connectivity and reconcile once a link is available.
- **System Integration & Data Contracts** — Shared, versioned payload schemas that keep firmware, backend, web, and mobile in agreement.

---

## Projects

| Repository | What it is |
| :--- | :--- |
| [kalasag](https://github.com/OctaCore-Technologies/kalasag) | Monorepo — relay firmware, coordination console, API server, field app, shared data contracts, and the project knowledge base |

### KALASAG

A low-cost, field-durable LoRa mesh relay system for disaster response. Relay nodes extend communication coverage into signal-dead areas, a coordination console guides the deploying team on where to place the next node, and a field companion app lets the responder register and position each node as it's dropped.

```
Relay Node (ESP32 + LoRa, mesh firmware)
   │  LoRa multi-hop mesh
   ▼
Gateway Node (internet-connected)
   │  MQTT / HTTP uplink
   ▼
Backend (Express + TypeScript)
   ├──► Web Console (React) — live coverage map, placement suggestions, node health
   └──► Field App (React Native) — BLE pairing, GPS/manual position logging, offline sync
```

---

## Teams

We split into three fronts, each owning a folder in the monorepo and its own integration branch.

| Team | Owns | Branch | Stack |
| :--- | :--- | :--- | :--- |
| [@OctaCore-Technologies/firmware](https://github.com/orgs/OctaCore-Technologies/teams/firmware) | `firmware/` | `firmware-main` | ESP32-S3, ESP-IDF, PlatformIO |
| [@OctaCore-Technologies/web](https://github.com/orgs/OctaCore-Technologies/teams/web) | `web/frontend/`, `web/backend/` | `web-main` | React, Vite, Express, TypeScript |
| [@OctaCore-Technologies/mobile](https://github.com/orgs/OctaCore-Technologies/teams/mobile) | `mobile/` | `mobile-main` | React Native, TypeScript |

`@OctaCore-Technologies/pm` and `@OctaCore-Technologies/qa` review every merge into `main`, enforced through CODEOWNERS.

---

## Members

| Name | Department | Role |
| :--- | :--- | :--- |
| **Aquino** | IoT | Scrum Master / Project Manager, Hardware, Quality Assurance |
| **Villareal** | IoT | Research Developer / Business Analyst, Quality Assurance (Lead), Hardware |
| **Seraspe** | IoT, Web App | Hardware (Lead), Backend Developer / Database Manager |
| **Tarroza** | IoT, Web App | Hardware, Frontend Developer |
| **Pangilinan** | Web App | Fullstack Developer |
| **Delos Santos** | Mobile App | Backend Developer / Database Manager (Lead) |
| **Gonzal** | Mobile App | Fullstack Developer |
| **Dayapera** | Mobile App | Frontend Developer |

---

## Contributing

Branch off a team integration branch, PR back into it, then team-main into `main` with PM and QA approval — full workflow in [CONTRIBUTING.md](https://github.com/OctaCore-Technologies/kalasag/blob/main/CONTRIBUTING.md).

---

*Software Engineering capstone team · BSCS-3A · Philippines*
