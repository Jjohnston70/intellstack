# Module Documentation Template Guide

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Templates for documenting Command modules

---

## Overview

Module documentation comes in two forms:
1. **Client-Facing** — Benefits-focused, non-technical
2. **Technical** — Implementation-focused, detailed

This guide provides templates for both.

---

## When to Create Module Documentation

- New Command module is built
- Existing module needs documentation
- Client needs to understand a module
- Technical team needs implementation reference

---

## Part 1: Client-Facing Module Documentation

### Purpose

Help clients understand what a module does and why it matters—without technical jargon.

### Template Structure

```markdown
# [module-name]

*[One-line tagline describing the benefit]*

---

## What This Module Does

[2-3 paragraphs explaining the module in plain language]

## Who It's For

[Bullet list of ideal users/situations]
- [Situation 1]
- [Situation 2]
- [Situation 3]

## Problems It Solves

[Bullet list in client voice]
- "[Problem statement 1]"
- "[Problem statement 2]"
- "[Problem statement 3]"

## Key Features

### [Feature 1 Name]
[What it does and why it matters]

### [Feature 2 Name]
[What it does and why it matters]

### [Feature 3 Name]
[What it does and why it matters]

## How It Works (Simple)

[Step-by-step explanation without technical details]

1. **[Step 1]** — [What happens]
2. **[Step 2]** — [What happens]
3. **[Step 3]** — [What happens]

## Integration with Other Modules

| Works With | What It Does Together |
|------------|----------------------|
| [module-name] | [Benefit] |
| [module-name] | [Benefit] |

---

*Part of the TNDS Command Center suite*
```

---

### Client-Facing Example: financial-command

```markdown
# financial-command

*Know which jobs make money—before month-end surprises.*

---

## What This Module Does

financial-command gives you real-time visibility into the money side of your operation. Instead of waiting for month-end reports to find out which jobs were profitable, you'll know as jobs close.

The module tracks job costs as they happen, automates invoice creation, and shows you profit margins before you're surprised by a bad month.

## Who It's For

- Operations with 5+ jobs per day
- Anyone who's been burned by unprofitable jobs they didn't catch
- Owners tired of chasing invoices days after jobs close
- Teams using ServiceTitan or similar dispatch software

## Problems It Solves

- "I don't know if a job was profitable until the accountant tells me"
- "Invoicing takes days because we're chasing down job details"
- "I can't tell which technicians are costing us money"
- "We're always finding unbilled work weeks later"

## Key Features

### Real-Time Job Costing
See costs accumulate as work happens—parts, labor, travel. No more surprises at month-end.

### Same-Day Invoicing
The moment a job closes, the invoice is ready. No chasing paperwork. No forgotten billables.

### Profitability Dashboard
One view showing which jobs made money, which didn't, and why. Spot patterns before they become problems.

## How It Works (Simple)

1. **Job closes** — Technician marks job complete in the field
2. **Costs calculated** — Parts, labor, and overhead automatically tallied
3. **Invoice triggered** — Invoice created and ready to send
4. **Profit visible** — See margin immediately on dashboard

## Integration with Other Modules

| Works With | What It Does Together |
|------------|----------------------|
| data-command | Pulls job data automatically |
| analytics-command | Feeds profitability reports |
| sms-command | Sends invoice notifications to customers |

---

*Part of the TNDS Command Center suite*
```

---

## Part 2: Technical Module Documentation

### Purpose

Provide implementation details for technical team—architecture, data model, configuration.

### Template Structure

```markdown
# [module-name] — Technical Documentation

**Version:** [X.X]
**Last Updated:** [Date]
**Status:** [Development / Production / Deprecated]

---

## Technical Overview

[High-level technical description]

### Purpose
[What problem it solves technically]

### Architecture Summary
[One paragraph describing technical approach]

---

## System Architecture

### Component Diagram

```
[ASCII or description of component relationships]
```

### Dependencies

| Dependency | Type | Purpose |
|------------|------|---------|
| [Dependency] | [Type] | [Why needed] |

---

## Data Model

### Entities

**[Entity Name]**
| Field | Type | Description |
|-------|------|-------------|
| [field] | [type] | [description] |

### Relationships

```
[Entity diagrams or relationship descriptions]
```

---

## API Integrations

### [Integration Name]

**Endpoint:** [URL pattern]
**Authentication:** [Method]
**Rate Limits:** [Limits]

**Key Operations:**
- [Operation 1]: [Description]
- [Operation 2]: [Description]

---

## Configuration

### Required Settings

| Setting | Type | Description | Default |
|---------|------|-------------|---------|
| [setting] | [type] | [description] | [default] |

### Environment Variables

```
[VAR_NAME]=value
```

---

## Testing

### Test Cases

| Test | Expected Outcome |
|------|-----------------|
| [Test scenario] | [Expected result] |

### Test Data Requirements

[What data is needed for testing]

---

## Troubleshooting

### Common Issues

**Issue:** [Problem description]
**Cause:** [Root cause]
**Solution:** [Fix steps]

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| [X.X] | [Date] | [Description] |
```

---

### Technical Example: financial-command

```markdown
# financial-command — Technical Documentation

**Version:** 1.2
**Last Updated:** January 29, 2026
**Status:** Production

---

## Technical Overview

### Purpose
Automate job costing calculations and invoice generation based on job completion events from dispatch systems.

### Architecture Summary
financial-command monitors job completion events via API webhooks, calculates costs using configurable formulas, and triggers invoice creation in connected accounting systems.

---

## System Architecture

### Component Diagram

```
┌─────────────────┐      ┌─────────────────┐      ┌─────────────────┐
│  ServiceTitan   │─────▶│ financial-      │─────▶│  QuickBooks     │
│  (Dispatch)     │      │ command         │      │  (Accounting)   │
└─────────────────┘      └────────┬────────┘      └─────────────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │  data-command   │
                         │  (Hub)          │
                         └─────────────────┘
```

### Dependencies

| Dependency | Type | Purpose |
|------------|------|---------|
| data-command | Internal | Central data store |
| ServiceTitan API | External | Job data source |
| QuickBooks API | External | Invoice destination |
| Google Apps Script | Runtime | Execution environment |

---

## Data Model

### Entities

**Job**
| Field | Type | Description |
|-------|------|-------------|
| job_id | String | ServiceTitan job ID |
| customer_id | String | Customer reference |
| status | Enum | open, in_progress, complete, invoiced |
| completed_at | DateTime | Job completion timestamp |

**JobCost**
| Field | Type | Description |
|-------|------|-------------|
| job_id | String | Parent job reference |
| labor_cost | Decimal | Calculated labor cost |
| parts_cost | Decimal | Parts total |
| overhead | Decimal | Applied overhead |
| total_cost | Decimal | Calculated total |
| margin | Decimal | Revenue - total_cost |

**Invoice**
| Field | Type | Description |
|-------|------|-------------|
| invoice_id | String | QuickBooks invoice ID |
| job_id | String | Source job reference |
| amount | Decimal | Invoice total |
| created_at | DateTime | Creation timestamp |
| sent_at | DateTime | Send timestamp (nullable) |

### Relationships

```
Job (1) ──── (1) JobCost
Job (1) ──── (0..1) Invoice
```

---

## API Integrations

### ServiceTitan API

**Base URL:** `https://api.servicetitan.io/v2/`
**Authentication:** OAuth 2.0 Bearer Token
**Rate Limits:** 100 requests/minute

**Key Operations:**
- `GET /jobs/{id}`: Fetch job details
- `GET /jobs?status=completed`: List completed jobs
- `GET /jobs/{id}/lineitems`: Fetch job line items

### QuickBooks API

**Base URL:** `https://quickbooks.api.intuit.com/v3/`
**Authentication:** OAuth 2.0
**Rate Limits:** 500 requests/minute

**Key Operations:**
- `POST /invoice`: Create invoice
- `GET /customer/{id}`: Verify customer exists

---

## Configuration

### Required Settings

| Setting | Type | Description | Default |
|---------|------|-------------|---------|
| labor_rate | Decimal | Hourly labor cost | 75.00 |
| overhead_pct | Decimal | Overhead percentage | 0.15 |
| auto_send_invoice | Boolean | Send invoice on creation | false |
| webhook_secret | String | ServiceTitan webhook validation | — |

### Environment Variables

```
SERVICETITAN_CLIENT_ID=xxx
SERVICETITAN_CLIENT_SECRET=xxx
QUICKBOOKS_CLIENT_ID=xxx
QUICKBOOKS_CLIENT_SECRET=xxx
```

---

## Testing

### Test Cases

| Test | Expected Outcome |
|------|-----------------|
| Job complete webhook received | JobCost record created |
| JobCost calculated | Margin = revenue - (labor + parts + overhead) |
| Invoice triggered | QuickBooks invoice created |
| Customer not in QuickBooks | Error logged, invoice queued |

### Test Data Requirements

- Sample job with line items
- Customer record in both systems
- Parts with costs

---

## Troubleshooting

### Common Issues

**Issue:** Invoice not created after job complete
**Cause:** Customer not found in QuickBooks
**Solution:** Check customer sync; create customer in QB first

**Issue:** Labor cost incorrect
**Cause:** labor_rate setting not updated
**Solution:** Update labor_rate in configuration

**Issue:** Webhook not received
**Cause:** Webhook URL not registered in ServiceTitan
**Solution:** Register webhook URL in ServiceTitan settings

---

## Changelog

| Version | Date | Changes |
|---------|------|---------|
| 1.2 | 2026-01-29 | Added overhead calculation |
| 1.1 | 2026-01-15 | QuickBooks integration |
| 1.0 | 2026-01-01 | Initial release |
```

---

## Module Documentation Checklist

### Client-Facing Checklist
- [ ] Tagline is benefit-focused
- [ ] No technical jargon
- [ ] Problems in client voice
- [ ] Features tied to benefits
- [ ] Integration table complete

### Technical Checklist
- [ ] Architecture diagram included
- [ ] Data model complete
- [ ] API details accurate
- [ ] Configuration documented
- [ ] Troubleshooting section helpful
- [ ] Version history maintained

---

**Document Status:** Active
**Next Review:** After 5 modules documented
**Feedback:** Note which sections teams find most useful

