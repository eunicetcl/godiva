# Project Godiva — AI-Driven Event Automation

Project Godiva is a service event automation platform that transforms operational signals (emails, alerts, system events) into structured decisions and controlled execution across customer channels.

## 🔗 Live Demo
[View Demo](https://godiva.vercel.app)

## How It Works

**Signal → AI Decision → Orchestration → LaunchDarkly → Channel (App / Web / Kiosk)**

- **Signal Intake** — captures events from email, monitoring systems, and operational inputs
- **AI Decision Layer** — interprets events, classifies severity, and recommends actions and SOPs
- **Execution Layer (LaunchDarkly)** — controls system behaviour through feature flags and bundles
- **Channel Layer** — applies changes consistently across App, UPortal, and Kiosk

## Build Tracks

| Track | Focus | Status |
|-------|-------|--------|
| Track 1 | LaunchDarkly Execution Control | ✅ Demo ready |
| Track 2 | AI Event Decisioning & Signal Intake | ✅ Demo ready |
| Track 3 | Operational Response & Traceability | ✅ Demo ready |
| Track 4 | Real-Time Customer Service Visibility | ✅ Demo ready |

### Track 1 — LaunchDarkly Execution Control
Runtime state controlled via predefined feature bundles. Each bundle groups related feature flags into a single coordinated action — one activation sets all dependent flags automatically. Requires a Maintenance/Event ID and human approval before execution.

### Track 2 — AI Event Decisioning & Signal Intake
Signal intake from email and monitoring systems. AI classifies event type, severity (MINOR / MAJOR / CRITICAL), and recommended action bundle using RAG-assisted classification against SOPs and prior cases.

### Track 3 — Operational Response & Traceability
Upon bundle activation, the platform automatically notifies the PIC via Microsoft Teams and Slack with full event context. Confluence incident pages, ServiceNow change tickets, and an audit trail are auto-generated — all linked to the same Service Event ID for end-to-end traceability.

### Track 4 — Real-Time Customer Service Visibility
Customer-facing banners update automatically across App, Web Portal, and Kiosk based on severity — no manual updates required.

| State | Banner |
|-------|--------|
| 🟢 Normal | No disruption |
| 🟡 Degraded | Partial service message |
| 🔴 Outage | Full outage banner |
| 🔵 Recovery | Service restored |

## Demo Scenarios

- 🔴 PayNow Gateway Failure (CRITICAL)
- 🟠 Scheduled Database Maintenance (MAJOR)
- 🟡 API Performance Degradation (MAJOR)
- 🟠 Mastercard Gateway Failure (MAJOR)

## Files

| File | Description |
|------|-------------|
| `incident-response-demo.html` | Main demo interface |
| `servicenow-ticket.html` | Mock ServiceNow change ticket |

---
AI-Driven Service Event Automation · Designed by Eunice Tan
