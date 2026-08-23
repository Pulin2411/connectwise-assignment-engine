# ConnectWise Assignment Engine

> Intelligent IT ticket assignment automation built with n8n and ConnectWise Manage.

## Overview

The ConnectWise Assignment Engine automates the process of identifying and routing ConnectWise service tickets to the appropriate support engineer.

The workflow combines ticket information with configurable assignment rules, engineer availability, shift schedules, exclusion rules, and support-level requirements to create a consistent and scalable ticket assignment process.

This project demonstrates how **n8n workflow automation** can be used to streamline IT Service Management operations and reduce manual ticket triage.

---

## Key Capabilities

- Automated ConnectWise incident retrieval
- Ticket normalization and processing
- Engineer availability evaluation
- Shift-based assignment handling
- Configurable exclusion rules
- Support-level based assignment
- Structured assignment decision logic
- Automated ConnectWise ticket updates
- Configuration-driven workflow behavior
- Designed for scalable IT support operations

---

## Architecture

```text
                    ┌──────────────────────┐
                    │    Schedule Trigger  │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Configuration & Rules│
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ ConnectWise Manage   │
                    │   Ticket Retrieval   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Ticket Normalization │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
       Exclusion Rules    Shift Schedule    Engineer Data
              │                │                │
              └────────────────┼────────────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ Assignment Decision  │
                    │       Engine         │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │ ConnectWise Ticket   │
                    │      Assignment      │
                    └──────────────────────┘
```

## Technology Stack

- **n8n** — Workflow automation
- **ConnectWise Manage** — IT service management
- **Google Sheets** — Configuration data
- **JavaScript** — Data transformation and business logic
- **REST APIs** — System integration

## Project Status

**Status:** Published n8n Workflow

The workflow has been implemented and published in n8n.

A sanitized version is included in this repository for portfolio demonstration and technical reference.

## Documentation

Detailed technical documentation is available in the `docs` directory.

## Author

**Pulin Shah**

IT Automation & AI Engineering
