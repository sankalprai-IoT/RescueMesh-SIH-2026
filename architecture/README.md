# RescueMesh — Architecture

RescueMesh is a connected disaster-response coordination platform designed to connect incident intelligence, command coordination, field response, and shelter operations through a unified system.

## Architecture Overview

The platform is organized into multiple functional layers that support disaster operations from risk intelligence through emergency response and shelter management.

The architecture follows a controlled and role-based operational model with clear separation between data processing, decision support, command actions, field response, and shelter operations.

---

## Core Architecture

```text
                    RESCUEMESH
                        │
        ┌───────────────┴───────────────┐
        │                               │
 PRE-DISASTER INTELLIGENCE        MID-DISASTER RESPONSE
        │                               │
        ▼                               ▼
 Data Sources                    Citizen SOS / Incident
        │                               │
        ▼                               ▼
 Data Verification               Area Resolution
        │                               │
        ▼                               ▼
 Risk Intelligence               Command Review
        │                               │
        ▼                               ▼
 Risk Analysis                   Field Assignment
        │                               │
        ▼                               ▼
 Decision Support                Field Verification
        │                               │
        ▼                               ▼
 Human Authorization             Incident Conversion
        │                               │
        └───────────────┬───────────────┘
                        │
                        ▼
                 SHELTER OPERATIONS
                        │
                        ▼
               RESIDENT ASSISTANCE

```

## System Architecture

RescueMesh follows a multi-layer software architecture that separates the user interface, API and security controls, core disaster-response engines, and persistent data storage.

```text
                         RESCUEMESH
                              │
                              ▼
                  ┌──────────────────────┐
                  │    FRONTEND LAYER    │
                  │ React 18 + Vite 6    │
                  │ Tailwind CSS         │
                  │ Leaflet / MapLibre   │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │ API & SECURITY LAYER │
                  │ FastAPI              │
                  │ JWT Authentication   │
                  │ Password Hashing     │
                  │ RBAC Middleware      │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │    CORE ENGINES      │
                  │ Multi-Factor Risk    │
                  │ Engine               │
                  │ Emergency SOS Engine│
                  │ Mesh Telemetry       │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │  PERSISTENCE LAYER   │
                  │ Relational Database  │
                  │ SQLite / PostgreSQL  │
                  │ System Audit Log     │
                  └──────────────────────┘
```
