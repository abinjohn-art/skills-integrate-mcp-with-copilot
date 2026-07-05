# Ready-to-create issues for repository

This file contains draft issue bodies you can copy-paste into GitHub Issues or use to create issues programmatically.

---

## Club discovery / searchable directory
**Description:** Add a searchable club directory with tagging, categories, and faceted search. Provide admin UI to create and manage club profiles (description, contact, tags, meeting times, links).

**Acceptance criteria:**
- Club list page with search and tag filters
- Club detail page with contact and membership info
- Admin UI to add/edit clubs

**Labels:** enhancement, needs-triage

---

## Recruitment / join workflows
**Description:** Implement member signup and join-request workflows for clubs, including join approval by club admins and role assignment (member, officer).

**Acceptance criteria:**
- Join request flow for authenticated users
- Club admin approval/rejection UI
- Automatic role assignment on approval

**Labels:** enhancement, needs-triage

---

## Events + ticketing (RSVPs & paid tickets)
**Description:** Add event pages with RSVP functionality, capacity limits, waiting lists, and paid ticket support (hosted checkout). Include attendee lists in admin UI.

**Acceptance criteria:**
- Event creation/editing UI
- RSVP and attendee management
- Ticket purchase flow wiring (webhook endpoint placeholder)

**Labels:** enhancement, needs-triage

---

## Payment integration (CyberSource hosted checkout)
**Description:** Integrate hosted checkout for paid tickets using CyberSource Secure Acceptance. Implement server-side generation of signed parameters and webhook/payment-complete endpoint to validate and record payments.

**Acceptance criteria:**
- Server endpoint to produce signed CyberSource params
- Frontend form POST to CyberSource (hosted checkout)
- Webhook endpoint to validate signature and process payments

**Labels:** enhancement, needs-triage

---

## OAuth / institutional SSO
**Description:** Add optional OAuth-based institutional SSO (Labs-style or similar) to allow users to authenticate with university accounts and prefill profile data.

**Acceptance criteria:**
- OAuth client configuration support
- Login/redirect flow and user provisioning on first login

**Labels:** enhancement, needs-triage

---

## React / Next.js frontend (progressive migration)
**Description:** Replace or augment current Flask templates with a modern React/Next.js frontend to improve UX, support SSR, and decouple frontend from backend API.

**Acceptance criteria:**
- Basic Next.js app scaffold in `frontend/`
- Example page consuming a backend API endpoint
- Documentation for running frontend and backend in development

**Labels:** enhancement, needs-triage

---

## Django REST API backend (add DRF layer)
**Description:** Add a Django + Django REST Framework API to expose club, event, and membership resources for use by the new frontend (or external clients).

**Acceptance criteria:**
- DRF endpoints for clubs, events, users, memberships
- Token-based or session authentication support
- API docs or OpenAPI schema

**Labels:** enhancement, needs-triage

---

## Webhook/dev payment flow (ngrok local testing)
**Description:** Add documentation and tooling for local webhook testing (ngrok or similar), and example env config for payment provider callbacks.

**Acceptance criteria:**
- `docs/ngrok-payment.md` with setup steps
- Example `.env` variables and local server instructions

**Labels:** enhancement, needs-triage

---

## CI / monitoring / storage integrations
**Description:** Add or standardize CI workflows, error monitoring (Sentry) configuration, and S3-compatible storage patterns for static and uploaded assets.

**Acceptance criteria:**
- Basic CI workflow (lint/test/build) in `.github/workflows/`
- Placeholder Sentry configuration and docs
- Storage abstraction documented (local vs S3)

**Labels:** enhancement, needs-triage

---

*If you want me to actually create GitHub Issues from these, provide a token with repo scope or enable an API that supports issue creation.*
