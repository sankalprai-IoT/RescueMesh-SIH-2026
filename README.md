# RescueMesh-SIH-2026

> A connected disaster-response coordination platform designed to bring incident intelligence, command coordination, field response, and shelter operations into one unified system.

**Team:** Didex  
**Project:** RescueMesh  
**Event:** Smart India Hackathon 2026

---

## Overview

During a disaster, information can become fragmented between incident reporting, command teams, field responders, and shelters.

**RescueMesh** is designed to connect these operational layers through a unified disaster-response platform.

The system follows a coordinated workflow:

**Incident → Intelligence → Command → Response → Shelter**

RescueMesh provides role-based operational interfaces so that different participants can access the functions relevant to their responsibilities.

---

## Core Response Workflow

```text
Incident Reporting
        ↓
AI Triage & Analysis
        ↓
Command Coordination
        ↓
Unit / Field Response
        ↓
Shelter Operations
        ↓
Resident Assistance
```
## Operational Roles

The platform is organized around different operational roles so that each participant can access the functions relevant to their responsibility.

| Role | Primary Responsibility |
|---|---|
| **Area Admin** | Area-level administration and operational oversight |
| **Commander** | Incident command and response coordination |
| **Unit Leader** | Unit-level operational coordination |
| **Responder** | Field-level response activities |
| **Shelter Manager** | Shelter-level management and coordination |
| **Shelter Responder** | Shelter-level operational assistance |

## Role-Based Operational Model

RescueMesh follows a role-based operational structure in which each participant works within a defined level of responsibility.

```text
                         RESCUEMESH
                             |
              +--------------+--------------+
              |                             |
        COMMAND LAYER                 SHELTER LAYER
              |                             |
         Area Admin                  Shelter Manager
              |                             |
          Commander                 Shelter Responder
              |
         Unit Leader
              |
          Responder

Each role operates within its defined responsibility while remaining part of the overall disaster-response workflow.
```

## Key Capabilities

### Incident Intelligence

- Incident reporting
- AI-assisted triage and analysis
- Emergency severity assessment
- Incident prioritization
- Operational information flow

### Command Coordination

- Incident command
- Response coordination
- Operational oversight
- Unit coordination
- Role-based dashboards

### Field Response

- Unit-level coordination
- Responder operations
- Field-level response activities
- Operational task handling

### Shelter Operations

- Shelter management
- Shelter coordination
- Shelter responder operations
- Resident assistance
- Shelter-level operational support

Demo

The repository contains dashboard demonstrations for the major operational roles supported by RescueMesh.

Available Role Demos
Area Admin
Commander
Unit Leader
Responder
Shelter Manager
Shelter Responder

Each role has its own dashboard demonstration showing the operational interface available to that role.

## Demo

The repository contains dashboard demonstrations for the major operational roles supported by RescueMesh.

### Available Role Demos

- **Area Admin** — Area-level administration and operational oversight
- **Commander** — Incident command and response coordination
- **Unit Leader** — Unit-level operational coordination
- **Responder** — Field-level response activities
- **Shelter Manager** — Shelter-level management and coordination
- **Shelter Responder** — Shelter-level operational assistance

Each role has its own dashboard demonstration showing the operational interface available to that role.

---

## Demo Video

🎥 **RescueMesh Full Demo**

[▶️ Watch the RescueMesh Demo](YOUTUBE_LINK_HERE)

---

## Role-wise Dashboard Demonstrations

| Role | Demo |
|---|---|
| **Area Admin** | View Demo |
| **Commander** | View Demo |
| **Unit Leader** | View Demo |
| **Responder** | View Demo |
| **Shelter Manager** | View Demo |
| **Shelter Responder** | View Demo |

## Architecture

The `architecture/` directory contains the architecture and system-design materials for RescueMesh.

It describes the major components of the platform and how information moves through the disaster-response workflow.

---

## Documentation

The `docs/` directory contains project documentation, technical references, workflows, and supporting materials.

---

## Presentation

The `presentation/` directory contains the official **RescueMesh — Smart India Hackathon 2026** presentation material.

## Repository Structure

```text
RescueMesh-SIH-2026/
│
├── architecture/
│   └── System architecture and design
│
├── demo/
│   ├── area-admin/
│   ├── commander/
│   ├── unit-leader/
│   ├── responder/
│   ├── shelter-manager/
│   ├── shelter-responder/
│   └── README.md
│
├── docs/
│   └── Project documentation
│
├── presentation/
│   └── SIH 2026 presentation
│
└── README.md
```
Project Workflow
                         INCIDENT
                            │
                            ▼
                 ┌────────────────────┐
                 │  AI TRIAGE &       │
                 │  ANALYSIS          │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │  COMMAND           │
                 │  COORDINATION      │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │  UNIT / FIELD      │
                 │  RESPONSE          │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │  SHELTER           │
                 │  OPERATIONS        │
                 └─────────┬──────────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │  RESIDENT          │
                 │  ASSISTANCE        │
                 └────────────────────┘
Team
Team Didex

Project: RescueMesh
Event: Smart India Hackathon 2026

RescueMesh is developed and maintained by Team Didex.

Project Status

🚧 RescueMesh is under active development.

The repository is being maintained as the project evolves toward the Smart India Hackathon 2026 submission and demonstration.

License

This project is developed by Team Didex for the Smart India Hackathon 2026.

RescueMesh

Incident → Intelligence → Command → Response → Shelter

Connecting disaster-response operations through one coordinated platform.
