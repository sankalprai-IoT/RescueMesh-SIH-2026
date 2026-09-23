# RescueMesh — Pre-Disaster Risk Intelligence Pipeline

The pre-disaster intelligence layer processes environmental and risk-related signals through a structured, sequential pipeline to support operational decision-making.

---

## Pipeline Overview

```text
External Data Sources
        │
        ▼
Data Adapters
(IMD / CWC / USGS / NDMA)
        │
        ▼
Quality Verification
        │
        ▼
Historical Memory
        │
        ▼
Risk Signals
        │
        ▼
Risk Scoring
(0–100)
        │
        ▼
Confidence & Delta Trend
        │
        ▼
Spatial Projection
(RFC 7946)
        │
        ▼
Spatial Exposure Analysis
        │
        ▼
Decision Support System
        │
        ▼
Human Authorization Gate
```
---

## Pipeline Stages

### 1. External Data Sources

Environmental and disaster-related observations are collected through configured data sources.

### 2. Data Adapters

Source-specific adapters normalize incoming information for downstream processing.

### 3. Quality Verification

Incoming data is checked before being used by subsequent processing stages.

### 4. Historical Memory

Relevant historical information is incorporated into the intelligence pipeline.

### 5. Risk Signals

Verified observations are transformed into operational risk signals.

### 6. Risk Scoring

Risk signals are processed into a normalized risk score on a `0–100` scale.

### 7. Confidence & Delta Trend

The system evaluates confidence and changes in risk conditions over time.

### 8. Spatial Projection

Risk information is projected into spatial representations using RFC 7946-compatible geometry.

### 9. Spatial Exposure Analysis

Spatial risk information is evaluated against exposed areas and relevant geographic context.

### 10. Decision Support System

The processed intelligence is presented as decision-support information for operational users.

### 11. Human Authorization Gate

Final operational authorization remains under human control before downstream action.

---

## Data Flow Boundary

The pipeline follows a unidirectional processing model. Downstream stages consume outputs from upstream stages without modifying upstream scores, geometries, or source-health states.
