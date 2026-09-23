# RescueMesh — Alert Authorization

The alert authorization layer provides a controlled workflow for reviewing and authorizing operational alerts before they are delivered to intended recipients.

---

## Authorization Workflow

```text
Risk / Decision Support
          │
          ▼
    Alert Candidate
          │
          ▼
     Human Review
       /      \
      ▼        ▼
  APPROVE    REJECT
      │
      ▼
 Alert Delivery
      │
 ┌────┼
 ▼    ▼    
IN-APP BROWSER 
```
---

## Authorization Stages

### 1. Risk / Decision Support

Processed risk or operational information is used to generate information that may require an alert.

### 2. Alert Candidate

The system prepares an alert candidate containing the relevant operational information.

### 3. Human Review

An authorized operator reviews the alert candidate before delivery.

### 4. Approval or Rejection

The authorized operator can approve or reject the alert candidate.

### 5. Alert Delivery

Approved alerts are delivered through the configured notification channels.

### 6. Delivery Channels

Depending on the configured workflow, alerts may be delivered through:

- In-App
- Browser
- Email
---

## Authorization Boundary

Alert delivery remains separated from the decision-support process.

Only an authorized user can approve an alert candidate for delivery. Rejected candidates do not proceed to the alert-delivery stage.
