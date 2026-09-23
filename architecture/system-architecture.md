# RescueMesh — System Architecture

RescueMesh follows a multi-layer software architecture that separates the user interface, API and security controls, core disaster-response engines, and persistent data storage.
---

## Architecture Layers

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
                  │     CORE ENGINES     │
                  │ Multi-Factor Risk    │
                  │ Engine               │
                  │ Emergency SOS Engine │
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
---

## Frontend Layer

The frontend provides the operational interfaces used by commanders, administrators, responders, and shelter teams.

- **React 18** — Frontend application framework
- **Vite 6** — Development and build tooling
- **Tailwind CSS** — Interface styling
- **Leaflet / MapLibre** — Spatial visualization
---

## API & Security Layer

The API and security layer handles application requests, authentication, authorization, and role-based access control.

- **FastAPI** — API and backend service layer
- **JWT Authentication** — Authenticated session and access control
- **Password Hashing** — Secure password storage
- **Role-Based Access Control (RBAC)** — Permission management based on operational roles
- **Area-Level Access Restrictions** — Controls access according to the user's operational area
---

## Core Engines Layer

The core engines process disaster intelligence and emergency-response operations.

- **Multi-Factor Risk Engine** — Processes disaster-related risk signals.
- **Emergency SOS Engine** — Handles emergency distress and SOS workflows.
- **Mesh Telemetry** — Supports connected field and operational data.
- **Incident & Response Processing** — Supports incident handling and response coordination.
- **Decision-Support Workflows** — Provides processed information for operational decision-making.

---

## Persistence Layer

The persistence layer stores operational data and maintains system records.

- **Relational Database** — Stores structured application and operational data.
- **SQLite** — Used for local deployment and development.
- **PostgreSQL** — Used for production deployment where applicable.
- **System Audit Log** — Maintains records of important system actions.

---

## Security Boundary

RescueMesh enforces authenticated and authorized access between operational areas.

Access to protected operations is controlled through authentication, role-based permissions, and applicable area-level restrictions.

Unauthorized cross-area actions are rejected by the API security layer.

---

## Architecture Summary

```text
Frontend
   ↓
API & Security
   ↓
Core Engines
   ↓
Persistence
```
