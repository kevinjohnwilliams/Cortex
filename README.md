# Cortex — Enterprise Data Management Platform

**Developer:** Kevin Williams  
**Organization:** Barrios Technology  
**Role:** Lead Developer & Architect  
**Stack:** Python · Django · JavaScript · MySQL · Git

---

## Overview

Cortex is a full-stack enterprise data management platform built to replace legacy SharePoint workflows. Designed and developed as the primary developer, Cortex provides a unified, SQL-backed interface for structured data management, workflow automation, and standardized reporting.

The platform serves as the backbone for managing program data in environments where data integrity, traceability, and access control are essential.

---

## Architecture

Cortex is built on an **Entity-Attribute-Value (EAV)** architecture, enabling dynamic, user-configurable data structures without requiring database migrations or developer intervention.

### Core Components

- **Dynamic Table System** — Users can create, configure, and manage custom data tables on the fly, replicating SharePoint-style list functionality with significantly more flexibility and control.
- **Custom Field Engine** — Supports multiple field types (Text, Number, Date, Boolean, Long Text) with calculated fields, formula evaluation, and conditional formatting rules stored as JSON.
- **Calculation Engine** — Safe formula evaluation for computed fields (e.g., `[Likelihood] × [Consequence]` for risk scoring).
- **AI-Assisted Features** — Integrated AI chat assistant with support for both cloud-based and local model inference, providing intelligent data entry suggestions and structured output interpretation.

---

## Key Features

- **SharePoint Replacement** — Fully replaces SharePoint list workflows with a modern, responsive web interface backed by relational database integrity.
- **Conditional Formatting** — User-defined color rules for numeric fields with cell and text styling options, giving users visual insight into their data without leaving the platform.
- **Data Export** — One-click export to CSV and Excel (.xlsx) with auto-generated filenames, supporting both full-table and filtered exports.
- **Dynamic Admin Interface** — Custom Django admin views that generate dynamically for each user-created table, with inline editing, filtering, and bulk operations.
- **Role-Based Access Control** — Permission tiers integrated with Django's auth framework, ensuring data governance and compliance with organizational security requirements.
- **Cross-Platform Reporting** — Companion Flutter application for automated report generation using predefined formats and validated data models.

---

## Technical Highlights

| Area | Detail |
|------|--------|
| **Backend** | Django with custom admin site, middleware, and modular app architecture |
| **Data Model** | EAV pattern via `CustomTable`, `CustomField`, `CustomEntry`, `CustomEntryValue` |
| **Frontend** | Django templates with responsive design, inline editing, and AJAX interactions |
| **AI Integration** | Embedded chat assistant with RAG capabilities and structured output suggestions |
| **Export** | Pandas + openpyxl for professionally formatted Excel output |
| **Version Control** | Git with feature branching (e.g., `cortex_change`, `feature/dynamic-update`) |

---

## Impact

- Consolidated fragmented SharePoint workflows into a single, reliable platform
- Reduced manual data processing and ad-hoc export requests
- Improved data accuracy through AI-assisted input validation
- Serves active programs in a high-criticality operational environment

---

## About

This repository serves as a portfolio reference for the Cortex platform. The source code is maintained on internal systems under Barrios Technology. For questions about the architecture, capabilities, or my contributions, feel free to reach out.

**Kevin Williams**  
Software Engineer — Barrios Technology  
M.S. Artificial Intelligence — University of Michigan
[GitHub](https://github.com/kevinjohnwilliams) · [Website](https://kevinjohnwilliams.github.io/)
