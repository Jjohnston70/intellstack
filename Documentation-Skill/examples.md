# TNDS Documentation Skill - Examples

## Example 1: Client-Facing Service Document

### Request
"Create a service document for Command Center Build"

### Output
A Word document with:
- TNDS logo in header
- Title: "Command Center Build"
- Subtitle: "Operational Visibility for 5-20 Person Operations"
- All sections filled with appropriate content
- Proper branding and formatting
- Saved as: `TNDS_Service_CommandCenterBuild_2026-01-26.docx`

---

## Example 2: Internal SOP

### Request
"Create an SOP for client onboarding after a signed agreement"

### Output
A Markdown document with:
- Title: "SOP: Client Onboarding"
- Effective date and version
- Purpose, scope, roles
- Step-by-step procedure
- Quality checks
- Related documents
- Revision history
- Saved as: `TNDS_SOP_ClientOnboarding_2026-01-26.md`

---

## Example 3: Diagnostic Cheat Sheet

### Request
"Create a cheat sheet for the ASSESS stage of Direction Protocol"

### Output
A Word document with:
- Title: "ASSESS Stage Diagnostic"
- Subtitle: "30-Minute Assessment Call"
- Before You Start section with setup and opening script
- Question sections with timing (10 min, 8 min, etc.)
- Red flags / Green flags checklists
- Next steps
- Saved as: `TNDS_Diagnostic_AssessStage_2026-01-26.docx`

---

## Example 4: Command Module Documentation

### Request
"Document the financial-command module for both clients and technical team"

### Output
TWO documents:

**Client-Facing** (`TNDS_Service_FinancialCommand_2026-01-26.docx`):
- What financial-command is
- Who it's for
- Problems it removes
- What you get
- Pricing (when part of Command Center)

**Technical Spec** (`TNDS_Spec_FinancialCommand_2026-01-26.md`):
- Technical architecture
- Data structure
- API integrations
- Implementation steps
- Testing approach

---

## Example 5: Proposal Document

### Request
"Generate a proposal for Peak HVAC based on our MAP session"

### Output
A Word document with:
- Cover page with TNDS branding
- Executive summary
- Current situation (from MAP)
- Proposed solution with diagrams
- Scope & deliverables
- Timeline
- Investment & payment terms
- Next steps
- Saved as: `TNDS_Proposal_PeakHVAC_2026-01-26.docx`

---

## Quick Commands Reference

| Say This | Get This |
|----------|----------|
| "Create service doc for [name]" | Client-facing service document |
| "Create SOP for [process]" | Standard operating procedure |
| "Create internal process doc for [topic]" | Internal how-to guide |
| "Create cheat sheet for [diagnostic]" | Assessment tool |
| "Document [module-name] module" | Module documentation |
| "Generate proposal for [client]" | Client proposal |
| "Create agreement for [service]" | Service agreement template |

---

## Template Content Examples

### Service Document Example Content

```python
content = {
    'what_this_is': [
        "Command Center Build transforms scattered operational data into real-time visibility. You'll see what's happening across your entire operation—jobs, crews, equipment, money—in one place.",
        "This isn't a dashboard you check once a week. It's a command center you use every day to make decisions, spot problems early, and actually know what's going on.",
        "We start with the Direction Protocol to understand your operation, then build exactly what you need using our Command modules. Fixed scope, fixed price. No open-ended projects."
    ],
    'who_this_is_for': [
        "5-20 person field service or office operations",
        "Owner is overwhelmed and can't see what's happening in real-time",
        "Information is scattered across texts, paper, spreadsheets, and memory",
        "Decisions are made blind because data arrives too late",
        "Can't take a day off without things falling apart",
        "Ready to invest in getting control of operations"
    ],
    'problems_removed': [
        "\"I find out about problems days after they happen\"",
        "\"I have no idea what our actual job costs are until it's too late\"",
        "\"Everything depends on me being available 24/7\"",
        "\"My dispatcher spends half the day playing phone tag\"",
        "\"We lose money on jobs and don't find out until month-end\"",
        "\"I can't trust the numbers I'm looking at\""
    ],
    'what_you_get': {
        'Central Data Architecture': [
            "All operational data in one place (not scattered across tools)",
            "Real-time sync between field and office",
            "Single source of truth everyone works from"
        ],
        'Custom Command Modules': [
            "Built specifically for your operation",
            "2-4 modules based on your MAP session",
            "Examples: financial-command, office-command, asset-command",
            "Integrated to work together seamlessly"
        ],
        'Team Training': [
            "Hands-on training for your team",
            "Documentation they can actually use",
            "Support during launch period"
        ]
    },
    'scope_pricing': {
        'investment': "$2,500 - $5,000 (determined during MAP stage based on complexity)",
        'timeline': "2-4 weeks from kickoff to launch",
        'payment_terms': "50% at project start, 50% at completion (or 40/30/30 for projects over $4,000)",
        'included': [
            "Direction Protocol (Identify, Assess, Map stages)",
            "Complete operational diagnostic and solution design",
            "Custom Command modules (2-4 based on needs)",
            "System setup and configuration",
            "Data migration and integration",
            "Team training and documentation",
            "30-day post-launch support"
        ],
        'not_included': [
            "Ongoing monthly support (see Command Partner)",
            "Additional modules beyond initial scope",
            "Hardware or third-party software licenses",
            "Changes to original scope (handled via change order)"
        ]
    },
    'prerequisites': [
        "Every engagement begins with the Direction Protocol: we Identify fit, Assess your situation, and Map your operation before we build anything.",
        "MAP stage required before pricing (90-120 minutes)",
        "Decision maker must be involved in MAP session",
        "Access to current systems and data during implementation"
    ],
    'what_comes_next': [
        "Most clients add Battle Rhythm Install to establish operating cadence",
        "Many move to Command Partner for ongoing support and optimization",
        "Additional Command modules can be added as needs evolve"
    ]
}
```

### SOP Example Content

```markdown
# SOP: Client Onboarding After Launch

**Effective Date**: 2026-01-26
**Version**: 1.0
**Status**: Active

## Purpose
Ensure every client has a smooth, consistent onboarding experience after signing the service agreement.

## Scope

**What This Covers**:
- Steps from signed agreement to project kickoff
- Initial setup and preparation
- Communication and expectation setting

**What This Doesn't Cover**:
- The Direction Protocol (covered in separate SOP)
- Technical implementation (covered in delivery SOPs)
- Post-launch support (covered in Command Partner SOP)

## Roles & Responsibilities

**Sales Lead (Jacob)**:
- Confirm payment received
- Send welcome email
- Schedule kickoff meeting
- Hand off to delivery team

**Delivery Lead**:
- Create project folder structure
- Set up project tracker
- Prepare kickoff agenda
- Conduct kickoff meeting

**Client**:
- Complete pre-kickoff questionnaire
- Attend kickoff meeting
- Provide system access as needed

## Procedure

### 1. Confirm Agreement and Payment
**Action**: Verify signed agreement received and deposit paid
**Who**: Sales Lead
**When**: Within 24 hours of client signing
**How**: 
1. Check for signed agreement in DocuSign
2. Verify payment received in QuickBooks
3. If missing, follow up immediately
**Output**: Confirmed in project tracker

### 2. Send Welcome Email
**Action**: Send welcome email with next steps
**Who**: Sales Lead
**When**: Same day as confirmation
**How**: Use "Client Welcome Email" template
**Output**: Email sent, logged in CRM

[Continue for all steps...]

## Quality Checks
- [ ] Signed agreement on file
- [ ] Payment received and logged
- [ ] Welcome email sent within 24 hours
- [ ] Kickoff scheduled within 3 business days
- [ ] Project folder created with correct structure
- [ ] Project tracker entry complete
- [ ] Client has access to shared workspace

## Exceptions
**When to Deviate**: Rush projects (2-week timeline)
**How to Handle**: Compress steps 2-4 into single day, same-day kickoff if possible
**Who Approves**: Sales Lead

## Related Documents
- Service Agreement Template
- Client Welcome Email Template
- Kickoff Meeting Agenda Template
- Project Tracker

## Revision History
| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | 2026-01-26 | Initial release | Jacob Johnston |
```

---

**END OF EXAMPLES**
