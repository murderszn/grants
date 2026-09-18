# AURABLOX — Active Project Portfolio

AURABLOX is a Delaware company operating as an AI transformation partner: 4 human employees and 8 agent employees (agents can spin up sub-agents). Services: data engineering, design, app development, writing, transcription, and AI teaching/enablement. Website: https://www.aurablox.com/

Below are the five active project areas — the work most likely to attract funding. Written for reuse in grant narratives and business plans.

---

## 1. NotSquat — AI equipment-utilization software for independent gyms

**The problem:** Once members pass the front desk, even attentive gym owners lose sight of how equipment is actually used — which racks sit idle, which benches are bottlenecks.

**The product:** Computer vision running on cameras the gym already owns. It distinguishes active lifting from rest and idle occupancy at each rack, bench, and machine, feeding a live operator dashboard. First product is aggregate and equipment-centered (not member tracking).

**Stage:** Core technical components built; integrating the live pipeline and validating with founding design-partner gyms (first partnership is no-cost).

**Repos** (under the `nrd-ai` org, co-maintained by Josh Johnson and Maurice Cadenhead):
- `nrd-ai/Not-Squat` — central engineering/CV/gamification/business hub
- `nrd-ai/Not-Squat-Detector-v0` — detection models
- `nrd-ai/NotSquat-Data-Warehouse` — telemetry warehouse (ClickHouse/Postgres)
- `nrd-ai/notsquat-marketing-site` — public site: notsquat.org
- `nrd-ai/notsquat-mobile-app` — Flutter mobile app

**Tech:** YOLOv11, MediaPipe, FastReID, OpenAPI backend spec, 16-bit gamification layer.

**Why it's fundable:** Real-world AI computer vision with a clear customer (independent strength gyms), a no-cost design-partner path to validation, and a physical-space data vision that extends beyond gyms.

---

## 2. Nameplate — asset & maintenance tracking for apartment portfolios

**The problem:** Apartment operators lose track of in-unit appliances — no lifecycle history, shrinkage, reactive maintenance, no repair-vs-replace economics.

**The product:** Every major appliance (fridges, ranges, washers, dryers, HVAC, water heaters) gets a tamper-evident scannable Nameplate Tag. Three surfaces:
- **Nameplate Field** (Flutter, offline-first) — technicians scan, inspect, and log service events even in signal-dead basements
- **Nameplate HQ** (React) — portfolio managers track asset lifecycle, dispatch work orders with SLA countdowns, analyze repair-vs-replace
- **Nameplate Portal** (React) — residents scan tags, file maintenance requests with photos, track appointments

**Stage:** Active development.

**Repo:** `murderszn/nameplate` (private)

**Tech:** Flutter, React + TypeScript, NestJS, PostgreSQL (Supabase), offline-first sync.

**Why it's fundable:** Proptech with a hardware+software wedge, clear ROI story for property managers (shrinkage prevention, maintenance economics), offline-first engineering for real field conditions.

---

## 3. Village — trusted recommendations for childcare & local services

**The problem:** Finding a trustworthy babysitter, house cleaner, or contractor still runs on scattered group-chat asks with no preserved context.

**The product:** A private recommendation network for childcare, household professionals, and local services through people you know. Preserves the missing context: who made the recommendation, what they hired the provider for, whether they'd hire again, and which formal checks have or haven't been completed. (Explicitly not a background-check product — the data model keeps those signals separate.)

**Stage:** Building — web app, API, and Flutter app in development.

**Repo:** `murderszn/Village` (private)

**Tech:** Flutter, Express API, MongoDB Atlas.

**Why it's fundable:** Trust-and-safety-first consumer product in the massive local-services market, with a differentiated data model around recommendation provenance.

---

## 4. Cerberus — security review for the AI-coded era

**The problem:** Developers now ship features in minutes with AI assistants — and security reviews can't keep up. Vibe-coded apps go live unaudited.

**The product:** Automated, zero-configuration security scanner and agent workbench. Three surfaces:
- **Deterministic scanner** — catalog-driven engine, runs identically in browser and CLI, scores repos 0–100
- **Agent CLI workbench** — nine named security-specialist personas that find and fix issues in a permission-controlled loop
- **GitHub App + cloud agent** — scan-grounded conversations, AI-generated fixes as one-click draft PRs

**Audiences:** vibe-coding founders (push-button audits), compliance leads (SOC 2 / HIPAA / GDPR prep), VC partners (rapid technical due diligence).

**Stage:** Active — CI green, cloud agent deployed.

**Repo:** `murderszn/cerberus` (public)

**Why it's fundable:** Directly addresses the security gap created by AI-assisted coding — a problem growing as fast as AI adoption itself. Clear paths to both developer-tool and compliance markets.

---

## 5. AURABLOX services — the engine behind it all

Client-facing AI transformation work: data engineering, design, application development, writing, transcription, and teaching companies to run their own AI environments. The 4-human + 8-agent structure is itself the proof of concept — a company operating at a scale far beyond its headcount through agent orchestration.

**Repo:** `murderszn/aurablox` (private) — site, relaunch campaign, training/enablement hub, agent skills.

---

## Entity & compliance notes for grant applications

- AURABLOX is set up as a **Delaware company**. Grant programs asking for a state business registration certificate (e.g., the Waukegan Microenterprise grant's "Business Registration Certificate – State of Illinois") will want the **Illinois foreign qualification (Certificate of Authority)** — verify this is in place before submitting.
- SAM.gov UEI registration is required for several programs; it's free at https://sam.gov — start early, processing takes time.
- Keep the "one application per business / one applicant per business" rules in mind — Joshua Johnson should be the named applicant everywhere.
