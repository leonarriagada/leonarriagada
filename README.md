# Leon Von Larkether
### Full-Stack Software Engineer & Application Architect
**Concepción, Chile** • [LinkedIn](https://linkedin.com/in/leonarriagada) • [Company Website](https://larkether.cl) • [Email](mailto:leonvonlarkether@gmail.com)

```text
Specializing in mission-critical web applications, high-concurrency database architecture, 
and enterprise API integrations with Next.js 16 (App Router), React 19, TypeScript, and Supabase / PostgreSQL.
```

---

## 🛠️ Core Technical Competencies

- **Frontend & Modern Web**: Next.js 16 (App Router, Turbopack), React 19, TypeScript, Tailwind CSS v4, Container Queries (`@container`), Responsive & Adaptive UI.
- **Backend & APIs**: Next.js Route Handlers, Node.js, Server-Side OAuth 2.0, Webhook Consumers, RESTful APIs.
- **Database & Concurrency**: PostgreSQL, Supabase, PL/pgSQL Atomic Operations, Exclusive Row-Level Locks (`FOR UPDATE`), Idempotency Patterns, Complex Migrations, Row-Level Security (RLS), RBAC.
- **Security & Cryptography**: AES-256-GCM Credential Vaults, SHA-256 PII Hashing, HTTP-only Anti-CSRF Cookies, Secure Session Management.
- **Quality & Testing**: Vitest (Unit & Integration Suites), Playwright (E2E), Automated CI pipelines.
- **Payment & Courier Integrations**: Webpay Plus (Flow.cl), Blue Express API, Starken Logistics.
- **Marketing & Attribution APIs**: Meta Marketing API v21.0, Meta Conversions API (CAPI Server-Side), Omnichannel Event Deduplication (`event_id`, `_fbp`, `_fbc`), GA4 & sGTM.

---

## 💼 Selected Commercial Case Studies

> [!NOTE]
> The source code for the client systems below is hosted in **private repositories under commercial Non-Disclosure Agreements (NDA)**. Technical architecture walkthroughs and live interactive demonstrations are available upon interview request.

### 1. SIGESPAI — Enterprise ERP & Financial Management Platform
* **Domain**: Heavy Equipment, Fleet Logistics & Industrial Services
* **Status**: `🔒 Private Production Repository`
* **Stack**: Next.js 16 • React 19 • Supabase (PostgreSQL) • PL/pgSQL • Vitest • Playwright
* **Architectural Highlights**:
  - **ACID Concurrency Engine**: Built atomic sequential voucher generation (COT, OC, IT) in `PL/pgSQL` utilizing row-level locks (`FOR UPDATE`) and idempotency keys to completely eliminate race conditions across simultaneous purchasing requests.
  - **Automated Bank Reconciliation**: Intelligent 1:N and N:1 reconciliation engine cross-referencing commercial bank statement imports against Chilean tax authority (SII RCV) records in CLP.
  - **Fine-Grained Security**: Multi-tenant Row-Level Security (RLS) policies and Role-Based Access Control (RBAC) audited with automated integration and E2E test suites.

---

### 2. NODO OS — Agency Operating System & Meta Marketing API Connector
* **Domain**: Marketing Automation, Project Governance & Digital Agency Operations
* **Status**: `🔒 Private Production Repository`
* **Stack**: Next.js 16 • TypeScript • Meta Marketing API v21.0 • Supabase • AES-256-GCM
* **Architectural Highlights**:
  - **Server-Side Meta OAuth 2.0 Pipeline**: Official Meta Marketing API connector handling CSRF validation through signed HTTP-only cookies and automatic 60-day token exchange.
  - **Cryptographic Credential Vault**: Zero-trust credential persistence using **AES-256-GCM** encryption (`v1:kid:iv:authTag:ciphertext`) inside an isolated, strictly-scoped database schema accessible only via backend service roles.
  - **Real-Time Client Portals**: Real-time KPI reporting dashboards and token-protected public report viewer links (`/reporte/[token]`) verified via SHA-256 signature checks.
  - **Adaptive Workspace**: Responsive task engine using CSS Container Queries (`@container`) with density toggling and live budget calculation.

---

### 3. Solventia — Investment Funnels & Server-Side Conversions Pipeline
* **Domain**: Real Estate Private Investment & FinTech
* **Status**: `🔒 Private Production Repository`
* **Stack**: Next.js • Node.js • Meta Conversions API (CAPI) • Supabase
* **Architectural Highlights**:
  - **Server-Side Event Pipeline (CAPI)**: Direct backend telemetry dispatch to Meta's Graph API, normalizing and hashing PII parameters (SHA-256) at the server layer to bypass ad-blockers and iOS privacy restrictions.
  - **Omnichannel Deduplication**: Zero-loss event synchronization pairing browser Pixel events with server CAPI payloads using deterministic `event_id` keys and cookie stitching (`_fbp`, `_fbc`).
  - **Algorithmic Lead Scoring**: Real-time risk/capital assessment engine segmenting high-net-worth investors before CRM dispatch.

---

### 4. Modular E-Commerce Monolith — Retail & Chilean Logistics
* **Domain**: Specialized Retail & Direct-to-Consumer
* **Status**: `🔒 Private Production Repository`
* **Stack**: Next.js 16 • PostgreSQL • Flow.cl (Webpay Plus) • Blue Express API • 39 Vitest Suites
* **Architectural Highlights**:
  - **Modular Domain Architecture**: Isolated domain modules for catalog management, shopping cart state, and order lifecycle backed by Supabase RLS.
  - **Chilean Payment & Logistics Integration**: Real-time shipping calculation with Blue Express and Starken couriers alongside atomic payment processing via Flow.cl Webpay Plus.
  - **Catalog Feed Automation**: Automated XML/JSON feed generators for Google Merchant Center, fully covered by 39 comprehensive Vitest suites.

---

### 5. Healthcare Diagnostic & Specialized Platforms
* **Healthcare Diagnostic Centers**: Scalable web portals for medical resonance facilities (*Resonancia Regional Concepción & Talcahuano*), optimizing appointment booking and clinical trust signals.
* **SaaS & Fleet Operations**: Logistics systems (*Grúas Paicaví*), capital investment portfolios (*Nordsee Capital*), and enterprise e-learning solutions (Moodle & SENCE regulatory compliance).

---

## 📐 Engineering Philosophy

1. **Concepts Over Frameworks**: Deep mastery of fundamental web standards, network protocols, ACID database transactions, and cryptographic primitives before abstractions.
2. **Deterministic Reliability**: Concurrency protection at the database level (`FOR UPDATE`, idempotency, transactions) instead of trusting client-side state.
3. **Defense in Depth**: Row-Level Security, strict boundary typing, zero-leak credential storage, and automated regression testing before deploying to production.

---

## 📬 Contact & Links

- **GitHub**: [github.com/leonvonlarkether](https://github.com/leonvonlarkether)
- **LinkedIn**: [linkedin.com/in/leonarriagada](https://linkedin.com/in/leonarriagada)
- **Email**: [leonvonlarkether@gmail.com](mailto:leonvonlarkether@gmail.com)
- **Company**: [larkether.cl](https://larkether.cl)
- **Location**: Concepción, Biobío Region, Chile
