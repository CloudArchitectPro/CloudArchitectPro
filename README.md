# Hi, I'm Naveen Madhavan 👋

I design and ship production SaaS platforms independently — directing AI-assisted development, but owning every architecture decision and outcome.

AWS-certified Cloud Security specialist (Security Specialty, Solutions Architect – Associate, Cloud Practitioner). Career-pivot builder — self-taught cloud/AWS since 2022, previously a decade in healthcare.

Most of my active work lives in **private repositories** — this profile is a summary of what's in them. Happy to walk through the code directly or grant reviewer access on request.

📫 cloud@naveen.cloud · [Personal Site](https://naveen.cloud) · [LinkedIn](https://linkedin.com/in/cloudarchitectpro) · Torrance, CA

---

## 🔒 What I've built (private repos)

### [Clouma Proof](https://clouma.com) — Compliance & GRC Automation Platform

Multi-tenant GRC platform automating compliance evidence collection and control mapping across SOC 2, HIPAA, PCI DSS, ISO 27001, NIST CSF, NIST 800-171/800-53, CMMC, and FedRAMP.

- Integrated the NIST 800-53 Rev 5.2 control catalog (1,014 controls) from official OSCAL source data, with a full evidence-collection and gap-analysis service layer
- Platform-admin console (Control Tower) shared across Proof and Shield — two-tier privilege model, instant session-kill switch, full audit-event logging
- OIDC/OAuth2 SSO (Google, Microsoft, LinkedIn, GitHub) with PKCE and just-in-time provisioning, plus passkey (WebAuthn) authentication across the shared identity platform
- Multi-tenant isolation via Postgres Row-Level Security (RLS)
- Stack: TypeScript, Node.js, PostgreSQL (Supabase), Domain-Driven Design

### [Clouma Shield](https://clouma.com) — CNAPP / Cloud Security Posture Platform

Cloud-native application protection platform providing continuous multi-cloud security scanning, drift detection, and auto-remediation. Built on the shared Clouma platform.

- Multi-cloud security scanning engine spanning AWS, Azure, GCP, OCI, and Kubernetes — AWS scanning live in production, additional provider connectors in active rollout
- Drift-detection pipeline hashing live findings against stored baselines on a continuous cron cadence
- Auto-remediation engine with a full approve/reject/rollback lifecycle for flagged findings
- Multi-cloud account onboarding, including kubeconfig ingestion for Kubernetes clusters
- Stack: TypeScript, Node.js, PostgreSQL (Supabase), Domain-Driven Design

### [IndxPro](https://indxpro.com) — AI-Assisted Stock Scanner (NSE, India)

Live production SaaS for Indian equity markets — momentum, mean reversion, volatility breakout, and smart-money scanning strategies, plus an AI signal-synthesis layer.

- Real-time market data integration (Upstox API)
- Broker-connected trade execution (manual-confirm, kill-switch gated)
- Stack: Next.js, TypeScript, PostgreSQL (Supabase), Vercel

### [JobPilot](https://jobs.naveen.cloud) — Job Search Automation Platform

Personal-use SaaS (Next.js, Vercel, Supabase/PostgreSQL with RLS, Cloudflare R2) automating end-to-end job search operations — built to solve my own job search, and open-sourced select components as a showcase.

- Multi-source job ingestion pipeline (Adzuna, Jooble, USAJOBS APIs) with dual-trigger scheduling and fingerprint-based deduplication across concurrent local + remote/international search queries
- AI-assisted resume/cover-letter tailoring engine (DeepSeek API) with strict fidelity guardrails — reconciliation logic reverts any AI-rewritten content where numeric claims diverge from the verified original
- Cloudflare R2 document storage layer with owner-scoped object keys, on-demand generation with signed-URL caching, and cache invalidation tied to content-regeneration events
- Postgres Row-Level Security across all tables for per-user data isolation

📂 [Showcase repo](https://github.com/CloudArchitectPro/jobpilot-showcase) — curated, redacted code samples demonstrating the architecture above (full app is private)

### distributed-sync-mesh — Geo-Distributed Infrastructure Lab

Zero-open-port, zero-trust file sync spanning two continents (USA + India, via a Raspberry Pi 5 relay).

- WireGuard/Tailscale mesh VPN, mutual authentication, encrypted transit
- Solved real-world CGNAT/NAT-traversal constraints
- 418,000 files / 21.7 GiB in continuous sync

### [AWS Security Exam Prep](https://scs.clouma.com) — examtraps / scs.clouma.com

Published two-volume AWS Security Specialty exam guide ("AWS SCS-C02: Exam Traps Decoded," 305 decoded exam scenarios) on Amazon, plus a companion SaaS platform with freemium access and integrated payments.

### [MedicalBrothers](https://medicalbrothers.com)

HIPAA-compliant healthcare staffing platform — in development, AES-256 encryption, audit logging, credentialing for 14 staff types.

---

## 🛠️ Core Skills

`AWS Security & IAM` `VPC` `KMS` `GuardDuty` `Terraform` `Docker` `PostgreSQL` `TypeScript/Node.js` `Multi-cloud (AWS/Azure/GCP/OCI)` `SOC2/HIPAA/PCI/ISO27001/NIST` `Zero-trust networking`

## 🎓 Certifications

- AWS Certified Security – Specialty (SCS-C02)
- AWS Certified Solutions Architect – Associate (SAA-C03)
- AWS Certified Cloud Practitioner (CLF-C01)
