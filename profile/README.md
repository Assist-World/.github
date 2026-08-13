<div align="center">

<!-- Replace with the hosted brand asset, e.g. https://assistworld.com/assets/logo-mark.svg -->
<img src="./assets/assistworld-logo.svg" alt="AssistWorld" width="180">

# AssistWorld

**Vetted virtual assistants for growing businesses.**

We match companies with trained, long-term virtual assistants — and we build the software that makes that matching fast, accountable, and measurable.

[Website](https://assistworld.com) · [Services](https://assistworld.com/services) · [Success Stories](https://assistworld.com/success-stories) · [Book a Consultation](https://assistworld.com/free-consultation)

</div>

---

## What we do

AssistWorld is a B2B virtual assistant staffing and placement company. We handle sourcing, vetting, onboarding, and ongoing management so our clients get a working assistant rather than a hiring project.

We support both generalist and specialised placements, including:

| Specialisation | Typical scope |
| --- | --- |
| **Executive & Administrative** | Inbox and calendar management, travel, research, reporting |
| **Legal** | Case intake, document prep, client correspondence, billing support |
| **IT & Technical** | Ticket triage, documentation, QA, vendor coordination |
| **Healthcare** | Scheduling, patient intake, records administration, follow-up |
| **Marketing & Operations** | CRM hygiene, content support, reporting, process documentation |

---

## What lives in this organisation

This org holds the engineering side of the business — the public web presence and the internal tooling our placement, sales, and marketing teams run on.

| Area | Description |
| --- | --- |
| **Web** | The AssistWorld marketing site and its supporting front-end applications |
| **Applications** | Standalone SPAs deployed at the edge and proxied under the main domain (e.g. the pricing calculator) |
| **Automation** | Integration layers connecting scheduling, CRM, and email systems into a single lead lifecycle |
| **Internal tooling** | Lead sourcing, enrichment, classification, and outreach systems used by the growth team |
| **Infrastructure** | Edge configuration, workers, routing, and deployment tooling |

Most repositories here are private. Public repositories, where they exist, are documented in their own READMEs.

---

## Engineering

### Stack

**Front-end** — React · Astro · Vite · WordPress + Elementor Pro · TypeScript · WebGL (Three.js, GLSL)

**Edge & infrastructure** — Cloudflare Pages · Workers · KV · WAF · self-hosted services on VPS via Coolify

**Data & backend** — Supabase (Postgres, RLS) · Airtable · Google Sheets

**Automation & lifecycle** — Zapier · Calendly · SuiteDash · Mailgun · Mailchimp

**Analytics & search** — GA4 · Google Search Console · Semrush

### Principles

- **Fail closed.** Security-relevant paths default to denial, not to best-effort. Row-level security and access rules are treated as part of the schema, not as an afterthought.
- **Independent paths over chained dependencies.** Automation branches run in parallel where possible so that one failure does not silently take down a sequence.
- **Attribution integrity is a first-class concern.** Tracking parameters, campaign tagging, and analytics configuration are reviewed as carefully as application code, because attribution damage is not retroactively fixable.
- **Document the constraint, not just the fix.** Platform limitations are recorded alongside the workaround so the next engineer inherits the reasoning.
- **Edge-first delivery.** Static and client-rendered surfaces are served from the edge and routed under a single origin for consistent caching, security, and analytics.

### Conventions

- Trunk-based development with short-lived feature branches.
- One logical change per commit; migrations are committed separately from application code.
- Conventional Commits for commit messages.
- Pull requests require review before merge. Infrastructure and schema changes require review from the owning engineer.
- Secrets live in environment configuration or the platform secret store — never in the repository, never in client bundles.

---

## Working with us

**Clients** — Start with a [free consultation](https://assistworld.com/getting-started) to scope the role, hours, and specialisation you need.

**Assistants** — We hire and train continuously. Applications are handled through our careers process on the main site.

**Engineers** — We work with a small, senior team across web, automation, and internal tooling. If that overlaps with what you do, get in touch.

---

## Contact

- **General** — hello@assistworld.com <!-- confirm before publishing -->
- **Security** — Please report suspected vulnerabilities privately to security@assistworld.com rather than opening a public issue. <!-- confirm this inbox exists -->
- **Web** — [assistworld.com](https://assistworld.com)

---

<div align="center">
<sub>© AssistWorld. All rights reserved.</sub>
</div>
