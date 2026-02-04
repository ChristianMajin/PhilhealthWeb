# SBAC Procurement Process

This document captures the process flow, roles, and user stories derived from the provided PDF/flowchart.

## Roles
- End-User
- BAC Secretariat
- TWG
- BAC
- Admin

## High-level Process
1. End-User Submits Request
2. BAC Secretariat checks documents
   - If incomplete → return to End-User
   - If complete → TWG review
3. TWG reviews technical specifications
   - If needs revision → return to End-User
   - If OK → BAC review
4. BAC reviews technical specifications
   - If not approved → return to End-User
   - If approved → TWG prepares bidding documents
5. TWG reviews bidding documents, revise if needed
6. BAC reviews bidding documents, revise if needed
7. Pre-procurement conference → Public bidding → Award of contract
8. Contract drafting, signing, NTP, posting & endorsement to COA & FMS
9. Completed

## User Stories / Acceptance Criteria
- As an End-User, I can submit a procurement request with title and specs. (AC: Request appears in dashboard with status "Submitted")
- As BAC Secretariat, I can mark submission as complete or return it as incomplete. (AC: Appropriate status and history recorded)
- As TWG, I can request revisions or pass to BAC for review. (AC: Status transitions accordingly)
- As BAC, I can approve or request compliance changes. (AC: Status transitions accordingly)
- As a workflow user, I can view a request's history with timestamps and actor names. (AC: History lists events)
- As a user, I can export CSV of request history. (AC: Downloadable CSV)
- Persistence is stored in browser localStorage to retain data between reloads.

## Testing / Quick Steps
1. Open `testtestSBAC.html` in a browser.
2. Click **Seed Sample Data** or create new request via **New Request**.
3. Click **Open** on a request and use **Act as** selector or **Login / Switch Role**.
4. Use **Next** and **Return** buttons to progress the request following the flowchart.
5. Export CSV to validate history export.

---

Notes: This is a prototype/demo. For production, replace localStorage with a backend API, add authentication, and implement file attachments and audit persistence.