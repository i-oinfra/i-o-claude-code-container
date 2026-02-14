# Integrated Ownership Infrastructure (I-O Infra)

Secure, transparent, and efficient land management and governance platform for The Gambia.

Developed by **Modou Sawo**.  
All rights reserved. Copyright © 2025 Modou Sawo.

Unauthorized use, reproduction, or distribution of this project, in whole or in part, without express written permission is strictly prohibited.

---

## Vision

To become the foundational platform for secure civic identity and property rights in The Gambia — building trust, reducing fraud, and unlocking economic potential through modern technology.

## Core Problems Addressed

- Dualistic land tenure system (formal leasehold vs. customary tenure) creating legal ambiguity
- Widespread fraud due to paper-based records and multiple sales of the same plot
- Extreme delays and inefficiency in paper-file movement between government departments
- No unified, authoritative, map-based national cadastre → frequent boundary disputes

## Core Principles

- **Security** – Cryptographically secure and immutable property records
- **Transparency** – Appropriate, role-based visibility for all stakeholders
- **Efficiency** – Reduce land transaction time from months to days
- **Accessibility** – Inclusive access (web + USSD/SMS for low-connectivity users)
- **Antifragility** – System becomes stronger from stress, disputes, and real-world usage

## Current Technical Foundation (MVP Stage)

- **Frontend**: React.js
- **Backend**: Node.js + Express.js
- **Database**: PostgreSQL
- **Mapping / Geospatial**: Mapbox
- **Blockchain / Ledger**: R3 Corda (permissioned DLT) – in progress
- **Desktop Client**: Tauri v2 (Rust) – planned for institutional & offline-first usage
- **Citizen Access Layer**: USSD & SMS gateway integration (planned)
- **Authentication**: JWT-based with role/portal-specific routing

## Key Features & Initiatives

### Foundational Workstreams

- **National Street Addressing System**  
  Physical addressing + digital mapping → base layer for national cadastre

- **Legacy Title Reconciliation**  
  Area-by-area process: data collection → geospatial survey → public display & adjudication → final on-chain issuance

### User Portals & Roles

- **Citizen Portal** – Manage property, request house numbers, verify titles
- **Government / Institutional Portals** – Ministry-specific dashboards (whitelabeled subdomains planned)
- **Professional Users** – Lawyers & Surveyors (verified against licensing bodies)
- **Platform Governance** – I-O Infra admins, adjudication committee, multi-signature consortium

### Core Workflows

- **Smart Deed** application – Guided, digital-first deed creation (like TurboTax)
- **Digital Wrapper** – Secure handling of scanned legacy documents with attestations
- **USSD/SMS Access** – `*777#`-style menu for basic queries and payments
- **Offline-First Institutional Mode** – Local Corda nodes with sync-on-reconnect
- **Emerald Green Protocol** – Branded desktop interface for government trust (#50C878 title bar)

### Antifragility Mechanisms (planned / in design)

- On-chain reputation system for professionals
- Dispute pattern learning & automated risk flagging
- Decentralized physical redundancy (QR-coded certificates)
- Governance CorDapp – rule changes via multi-signature consortium vote

## Available Scripts (Frontend & Development)

```bash
# Start backend server (Express API)
node server.js

# Start frontend development server (hot reload)
npm start

# Build production frontend
npm run build

# Compile component-specific SCSS
npm run build-css
npm run build-css-layout
npm run build-css-searchResults
npm run build-css-addAPlace
npm run build-css-map

# Run tests (Jest)
npm test