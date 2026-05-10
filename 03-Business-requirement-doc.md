# Business Requirements Document (BRD) - Rental Platform

## What is a BRD?
A Business Requirements Document (BRD) is a formal document that describes the **business needs** and **expected outcomes** of a project from a business perspective (not a technical one). It answers: **"What does the business need?"** and **"Why do we need it?"**

For your rental platform, the BRD focuses on solving the real problems (lack of trust, manual processes, disputes) and achieving business goals (ease of use, transparency, fair resolution).

---

## Core Contents of a BRD for the Rental Platform

### 1. Executive Summary
- One-page overview of the entire project.
- **What:** A platform to automate rental processes (apartments, shops, villas, rooms).
- **Why:** To solve current market problems (no search platform, untrustworthy brokers, disputes, lack of documentation).
- **Who:** Tenants, Owners, Brokers, Platform Admins.
- **How:** Platform acts as a trusted intermediary for a fee paid by the property owner.

### 2. Business Objectives & Success Criteria
What does the business want to achieve? How to measure success?

| Objective | Success Metric (KPI) |
|-----------|----------------------|
| Reduce search time for tenants | Average time from search to booking < 3 days |
| Reduce disputes between parties | Dispute rate < 5% of total contracts |
| Increase trust | 90% of users complete identity verification |
| Ensure fair move-in/move-out | 100% of rentals have documented condition report |
| Platform revenue | 500+ active properties within first year |

### 3. Project Scope
#### In-Scope (What the platform will do):
- User registration and identity verification (tenant, owner, broker).
- Property listing and search.
- Digital contract signing.
- Payment collection (rent, deposit, fees).
- Condition documentation (photos/videos at move-in and move-out).
- Maintenance request tracking.
- Review and rating system.
- Dispute resolution workflow.

#### Out-of-Scope (What the platform will NOT do in first version):
- AI-based pricing recommendations.
- Complex maps and geolocation.
- Smart contract automation via blockchain.
- Integration with government property registries (if not available).
- Multi-language support beyond Arabic.

### 4. Stakeholders & Users (Actors)
Detailed profiles of who will use the platform.

| Actor | Primary Need | Pain Point Solved |
|-------|--------------|-------------------|
| Tenant (Sami) | Find and rent a property easily | No search platform, fear of scams, disputes at move-out |
| Owner | Rent property safely with guaranteed income | Fear of damage, late payments, no documentation |
| Broker | Manage properties and clients | Disorganized process, untrustworthy reputation |
| Platform Admin | Monitor and regulate the market | Lack of oversight, no data |

### 5. Business Rules
These are the rules that govern how the platform operates (non-negotiable from a business perspective).

**Examples:**
- A property cannot be listed without owner identity verification.
- A contract cannot be signed without both parties verifying their identity.
- A tenant cannot move in without documenting the property condition (photos/videos).
- A deposit cannot be released without a joint move-out inspection.
- An owner cannot evict a tenant without following the platform's dispute resolution process.
- The platform fee is paid by the owner only upon successful contract signing.
- A tenant with a low rating (below 2 stars) must pay a higher deposit.

### 6. Functional Requirements (Business View)
What the system must **do** from a business perspective (not technical implementation).

| Requirement ID | Description (Business Language) |
|----------------|----------------------------------|
| BR-FR-01 | The platform shall allow a tenant to search for properties by city, price, type, and number of rooms. |
| BR-FR-02 | The platform shall allow an owner to add, edit, or hide a property listing. |
| BR-FR-03 | The platform shall require identity verification for both tenant and owner before a contract is signed. |
| BR-FR-04 | The platform shall provide a digital contract template that both parties sign electronically. |
| BR-FR-05 | The platform shall allow the tenant to upload photos/videos of the property at move-in and move-out. |
| BR-FR-06 | The platform shall hold the security deposit in escrow (or track it) until move-out is complete. |
| BR-FR-07 | The platform shall notify both parties 7 days before rent is due. |
| BR-FR-08 | The platform shall allow a tenant to report a maintenance issue and track its status. |
| BR-FR-09 | The platform shall allow both parties to rate each other after the contract ends. |
| BR-FR-10 | The platform shall provide an admin dashboard to monitor listings, users, and disputes. |

### 7. Non-Functional Requirements (Quality Attributes)
How well the system performs.

| Requirement ID | Description |
|----------------|-------------|
| BR-NFR-01 | The platform must be available 99.9% of the time (reliable). |
| BR-NFR-02 | Search results must appear within 3 seconds. |
| BR-NFR-03 | All personal data and documents (IDs, contracts) must be encrypted. |
| BR-NFR-04 | The platform must work on mobile phones (responsive design or app). |
| BR-NFR-05 | The platform must support Arabic language fully. |
| BR-NFR-06 | Payment processing must be secure and PCI-compliant (or equivalent locally). |

### 8. Assumptions & Constraints
#### Assumptions (Things we believe to be true):
- Tenants and owners have basic smartphone/computer literacy.
- There is enough demand for rental properties in target cities (Taiz, Sana'a, Aden).
- Payment gateways or local banking alternatives are available.
- Users are willing to pay a platform fee (owner) and provide identity documents.

#### Constraints (Limitations):
- Legal framework for e-signatures may not be fully established in Yemen.
- No central property registry to verify ownership easily.
- Limited internet penetration in some areas.
- Many users prefer cash over digital payments initially.

### 9. Business Risks & Mitigation
| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|-------------|
| Owners refuse to pay platform fee | High | High | Offer free trial period, show value (protection, fewer vacancies) |
| Tenants don't trust digital contracts | Medium | Medium | Allow printing contracts, partner with local notaries |
| Payment integration fails | Medium | High | Start with cash collection points or mobile wallets |
| Fake property listings | High | High | Manual approval for first listings, plus owner verification |
| Disputes still happen offline | Medium | Medium | Require all communication and evidence via platform |

### 10. Business Process Flows (High Level)
Simple diagrams or step-by-step descriptions of key processes.

**Example: Rental Lifecycle (Business View)**
1. Owner adds property → Admin verifies → Listing goes live.
2. Tenant searches → Finds property → Requests visit.
3. Owner accepts visit → Tenant views property.
4. Tenant agrees → Both sign digital contract → Tenant pays deposit + first rent.
5. Tenant moves in → Documents condition (photos).
6. Tenant pays monthly rent via platform.
7. Tenant moves out → Joint inspection → Deposit returned or disputed.
8. Both parties rate each other.

### 11. Key Performance Indicators (KPIs) for Business
- Number of active listings.
- Number of successful contracts signed per month.
- Average time to rent a property (listing to contract).
- Dispute rate (% of contracts with formal dispute).
- User satisfaction score (post-rental survey).
- Platform revenue (fees collected).

### 12. Budget & High-Level Timeline (Optional but often included)
| Phase | Duration | Estimated Cost |
|-------|----------|----------------|
| Requirements & Design | 1 month | $X |
| MVP Development | 3 months | $X |
| Beta Testing | 1 month | $X |
| Launch & Marketing | 1 month | $X |

### 13. Glossary (Terms)
| Term | Definition |
|------|-------------|
| Tenant | The person renting the property. |
| Owner | The person who owns the property. |
| Deposit (Guarantee) | Money held as security against damages or unpaid rent. |
| Escrow | Holding money in a neutral account (platform) until conditions are met. |
| Move-in Inspection | Documenting the property condition when tenant enters. |
| Move-out Inspection | Documenting the property condition when tenant leaves. |

---

## BRD vs Other Documents (Quick Clarification)

| Document | Purpose | Audience |
|----------|---------|----------|
| **BRD (Business Requirements Document)** | What the business needs and why | Business stakeholders, executives, project sponsors |
| **FRD / FRS (Functional Requirements Specification)** | Detailed system behavior | Development team, QA |
| **SRS (Software Requirements Specification)** | Technical details (APIs, databases) | Developers, architects |
| **MVP Scope** | What features in first release | Product manager, team |

---

## Example: One BRD Requirement Written Properly

**Requirement ID:** BR-FR-05 (Condition Documentation)

**Description:**
The platform shall allow the tenant to upload photos and videos of the property at move-in and move-out.

**Business Justification:**
Currently, disputes happen because there is no record of the property's condition. Without documentation, owners falsely accuse tenants of damage to keep the deposit. With a visual record, both parties are protected, and disputes decrease by an estimated 70%.

**Acceptance Criteria (Business View):**
- Tenant can upload up to 20 photos and 3 videos at move-in.
- Owner can view and confirm or dispute the uploads within 48 hours.
- Same process applies at move-out.
- All media is timestamped and stored for 12 months after contract ends.

**Dependencies:**
- Storage service (cloud) must be available.
- User must have a smartphone camera.

---

## Summary Checklist for Your BRD

- [ ] Executive Summary
- [ ] Business Objectives & Success Metrics (KPIs)
- [ ] Project Scope (In/Out)
- [ ] Stakeholders & Users
- [ ] Business Rules
- [ ] Functional Requirements (Business view)
- [ ] Non-Functional Requirements
- [ ] Assumptions & Constraints
- [ ] Business Risks & Mitigation
- [ ] High-Level Process Flows
- [ ] KPIs for Business
- [ ] Budget & Timeline (if needed)
- [ ] Glossary