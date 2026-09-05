# OctaCore Technologies

An eight-person software engineering team building **KALASAG** — a low-cost, field-durable LoRa mesh relay system for disaster response.

Relay nodes extend communication coverage into signal-dead areas, a coordination console guides the deploying team on where to place the next node, and a field companion app lets the responder register and position each node as it's dropped.

## Projects

| Repository | What it is |
| :--- | :--- |
| [kalasag](https://github.com/OctaCore-Technologies/kalasag) | Monorepo — relay firmware, coordination console, API server, field app, shared data contracts, and the project knowledge base |

## How KALASAG fits together

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

## Teams

We split into three fronts, each owning a folder in the monorepo and its own integration branch.

| Team | Owns | Branch | Stack |
| :--- | :--- | :--- | :--- |
| [@OctaCore-Technologies/firmware](https://github.com/orgs/OctaCore-Technologies/teams/firmware) | `firmware/` | `firmware-main` | ESP32-S3, PlatformIO, Meshtastic/MeshCore |
| [@OctaCore-Technologies/web](https://github.com/orgs/OctaCore-Technologies/teams/web) | `web/frontend/`, `web/backend/` | `web-main` | React, Vite, Express, TypeScript |
| [@OctaCore-Technologies/mobile](https://github.com/orgs/OctaCore-Technologies/teams/mobile) | `mobile/` | `mobile-main` | React Native, TypeScript |

`@OctaCore-Technologies/pm` and `@OctaCore-Technologies/qa` review every merge into `main`, enforced through CODEOWNERS.

## Members

| Name | Department | Role |
| :--- | :--- | :--- |
| **Aquino** | IoT | Hardware, QA, Scrum Master / Project Manager |
| **Villareal** | IoT | Hardware, QA (Lead), Research Developer / Business Analyst |
| **Seraspe** | IoT, Web | Hardware (Lead), Backend Developer / Database Manager |
| **Tarroza** | IoT, Web | Hardware, Frontend Developer |
| **Pangilinan** | Web | Backend Developer / Database Manager, Frontend Developer |
| **Delos Santos** | Application | Backend Developer / Database Manager (Lead) |
| **Gonzal** | Application | Fullstack Developer, Frontend Developer |
| **Dayapera** | Application | Frontend Developer |

## Stack

**Core**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=for-the-badge&logo=nodedotjs&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)

**Web**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)

**Mobile**

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

## Contributing

Branch off a team integration branch, PR back into it, then team-main into `main` with PM and QA approval — full workflow in [CONTRIBUTING.md](https://github.com/OctaCore-Technologies/kalasag/blob/main/CONTRIBUTING.md).

---

*Software Engineering capstone team · BSCS-3A · Philippines*
