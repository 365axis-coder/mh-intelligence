MH-Intelligence System
Strategic Operations Platform — Maya Hotait Advisory

Transformation is not an initiative. It is architecture.


About This System
MH-Intelligence is a private, purpose-built operations system designed and developed for Maya Hotait Advisory — a Strategic Transformation Advisory practice operating across MENA, Africa, and Eurasia.
This is not an off-the-shelf tool. It is a customized workflow system built from the ground up to reflect how Maya Hotait thinks, works, and delivers — structured around the philosophy that credibility is engineered, not communicated.

What It Does
The system operates across three integrated modules:
🧾 Billing

Invoice management with multi-currency support (USD · AED · SAR · EUR · GBP · LBP)
Payment tracking and receipt generation
Official Invoice, Receipt Voucher, and Proposal templates — print-ready PDF

📁 Project Management

Full project lifecycle: Proposal → Contract → Kickoff → Assessment → Planning → Delivery → Handover → Closure
Custom phases and sub-phases per project
Task management with status, priority, assignee, and due dates
Gantt Chart timeline view
WIP Reports and Final Project Reports

📊 Dashboard

Real-time overview: invoiced, collected, outstanding, active projects
Task status circle chart
Progress by phase type
Overdue task alerts


Technical Stack
LayerTechnologyFrontendVanilla HTML · CSS · JavaScript (no framework)DatabaseSupabase (PostgreSQL)AuthSupabase anon key (single-user)HostingGitHub PagesDocumentsPrint-to-PDF via browserStorageSupabase cloud + localStorage fallback
No dependencies. No npm. No build step. A single HTML file that runs anywhere.

Architecture Philosophy
This system was intentionally built as a single HTML file for a reason:

Zero setup — open and use
No server required
Works on any device, any browser
Fully portable — the entire system is one file
Data persists in Supabase cloud — accessible from any device

The database schema is designed for future scalability:

Multi-client ready
Supabase Row Level Security enabled
Migration path to multi-user when needed


Database Schema
settings        → company profile, consultants, bank details
invoices        → client invoices with line items (JSONB)
payments        → payment records linked to invoices
projects        → project metadata and contract values
project_phases  → phases per project with dates
sub_phases      → sub-phases within phases
tasks           → tasks linked to phases or sub-phases

Document Templates
Three official document templates are integrated and auto-populated from system data:

Invoice — MH-INV-[YEAR]-[XXX]
Receipt Voucher — MH-RCV-[YEAR]-[XXX]
Strategic Advisory Proposal — MH-PROP-[YEAR]-[XXX]

All templates carry the MH brand identity, are editable before printing, and export as professional PDFs.

Personal Notes
This system was built because no existing tool matched the way I work.
Most CRMs and project management tools are built for teams, for products, for volume. My work is different — it's advisory, relational, and deeply contextual. Every client engagement is unique. Every project has its own architecture.
I needed a system that:

Reflects my workflow, not a generic template
Keeps billing and project management in one place
Generates professional documents without extra tools
Stores data securely without depending on expensive subscriptions
Works on my phone in the field, not just at my desk

This is that system.
It started as a simple billing tracker. It became an intelligence system — because that is what the work demands.

Roadmap

 Client portal (view-only access for clients)
 Email notifications for overdue tasks
 Document attachments per phase
 Multi-user access (when team scales beyond 10 clients)
 Mobile app wrapper (PWA)


About Maya Hotait
Maya Hotait is an Organizational Transformation and Financial Strategy Advisor operating across MENA · Africa · Eurasia.
She advises boards, executive leadership, and decision-makers on designing institutions that are structurally sound, financially resilient, and governance-driven.
CVA · CFIP · CIFE · ISO 45001 Lead Auditor (CQI IRCA) · CSP · MBA
www.mayahotait.com

Because institutions that endure are not managed. They are deliberately architected.
