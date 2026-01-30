# TNDS DOCUMENTATION SKILL
## User Manual

**Version**: 1.0  
**Effective Date**: January 26, 2026  
**Owner**: Jacob Johnston  
**Contact**: 719-204-6365 | jacob@truenorthstrategyops.com

---

## TABLE OF CONTENTS

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Basic Usage](#basic-usage)
4. [Document Types Guide](#document-types-guide)
5. [Step-by-Step Tutorials](#step-by-step-tutorials)
6. [Brand Guidelines Reference](#brand-guidelines-reference)
7. [Template Reference](#template-reference)
8. [Advanced Features](#advanced-features)
9. [Troubleshooting](#troubleshooting)
10. [Best Practices](#best-practices)
11. [FAQ](#faq)
12. [Appendix](#appendix)

---

## INTRODUCTION

### What is the TNDS Documentation Skill?

The TNDS Documentation Skill is an AI-powered document generation system that creates professionally branded materials following True North Data Strategies' established voice, structure, and visual identity.

**Think of it as**: Your in-house documentation specialist who knows the TNDS brand inside and out, can write in the TNDS voice perfectly, and formats everything to spec—every single time.

### What Can It Do?

**Client-Facing Documents**:
- Service descriptions and offering sheets
- Professional proposals
- Service agreements and contracts
- Engagement overviews
- Presentations

**Internal Documents**:
- Standard Operating Procedures (SOPs)
- Process documentation
- Team training materials
- Diagnostic cheat sheets
- How-to guides

**Technical Documents**:
- Technical specifications
- System architecture docs
- API documentation
- Implementation guides

### Why Use This Skill?

**Consistency**: Every document uses the same voice, tone, and branding  
**Speed**: Generate a complete branded document in minutes, not hours  
**Quality**: Built-in quality checks ensure professional results  
**Scalability**: Easily create dozens of documents without variation  
**Professionalism**: Clients see polished, cohesive materials every time

### Who Should Use This Manual?

- **Jacob**: Primary user, creating all document types
- **Team members**: Anyone who needs to create TNDS documentation
- **Future employees**: Onboarding resource for maintaining brand consistency
- **Contractors**: External help creating TNDS materials

---

## GETTING STARTED

### Prerequisites

Before using the skill, ensure you have:

1. ✅ Access to Claude (claude.ai or Claude Desktop)
2. ✅ The TNDS Documentation Skill files in your environment
3. ✅ TNDS logo file (word-doc-tnds-logo.png)
4. ✅ Basic understanding of TNDS services (Direction Protocol, Command Protocol)

### Installation

**Option 1: Use in Claude.ai (Recommended)**

1. Upload the skill files to your conversation with Claude
2. Reference the skill when you need a document:
   ```
   "Using the TNDS Documentation skill, create a service document for..."
   ```

**Option 2: Claude Desktop with MCP**

1. Copy `tnds-documentation-skill` folder to your MCP skills directory
2. Claude will auto-detect it
3. Reference by name in conversations

**Option 3: Keep in Your Workspace**

1. Store all files in Google Drive or Notion
2. Upload when needed for document creation
3. Keep for reference and team training

### Verification

Test the skill is working:

```
"Create a simple test document to verify the TNDS Documentation skill is working"
```

You should receive:
- A Word or Markdown document
- Properly formatted with TNDS branding
- A download link

If successful, you're ready to go!

---

## BASIC USAGE

### The Simple Pattern

Creating any TNDS document follows this pattern:

```
1. Tell Claude what type of document you need
2. Provide the necessary context/information
3. Specify output format (Word or Markdown)
4. Review and refine if needed
5. Download the final document
```

### Your First Document

Let's create a simple service document:

**Step 1**: Start the conversation
```
"Using the TNDS Documentation skill, create a service document for Command Center Build"
```

**Step 2**: Claude will ask clarifying questions if needed
```
Claude: "I'll create a service document for Command Center Build. Should I use the standard template or do you have specific customizations?"

You: "Use the standard template"
```

**Step 3**: Claude generates the document
```
Claude: [Creates Word document with full branding]
- Applies TNDS logo
- Uses correct colors and fonts
- Fills all sections
- Saves with proper filename
```

**Step 4**: Review the document
```
Claude: "I've created TNDS_Service_CommandCenterBuild_2026-01-26.docx. 
[Download link]

Would you like me to adjust anything?"
```

**Step 5**: Refine if needed
```
You: "Make the 'Who This Is For' section more concise"

Claude: [Updates document and provides new download link]
```

That's it! You've created your first TNDS document.

### Quick Command Reference

Use these shortcuts for common requests:

| You Say | Claude Creates |
|---------|---------------|
| "Create service doc for [X]" | Client-facing service document |
| "Create SOP for [X]" | Standard operating procedure |
| "Create process doc for [X]" | Internal process guide |
| "Create cheat sheet for [X]" | Diagnostic tool |
| "Generate proposal for [client]" | Client proposal |
| "Document [module] module" | Module documentation |

---

## DOCUMENT TYPES GUIDE

### Client-Facing Service Documents

**Purpose**: Describe a service offering to potential clients

**When to Use**:
- Explaining Command Center Build
- Explaining Battle Rhythm Install
- Explaining Command Partner
- Documenting new service offerings
- Creating sales collateral

**Output Format**: Word document (.docx) with full branding

**Typical Sections**:
1. Title and subtitle
2. What This Engagement Is
3. Who This Is For
4. Problems This Removes
5. What You Get
6. Scope & Pricing
7. Prerequisites
8. What Comes Next

**Example Request**:
```
"Create a service document for Command Partner. 
Price is $1,000-$2,000/month for ongoing ops support.
This is selective - only offered to proven clients."
```

**What You'll Get**:
- 3-5 page Word document
- TNDS logo in header
- All sections properly formatted
- Navy and Teal branding throughout
- Professional footer with contact info
- Filename: `TNDS_Service_CommandPartner_[date].docx`

---

### Internal Process Documents

**Purpose**: Document how the team executes a process

**When to Use**:
- Training new team members
- Standardizing workflows
- Documenting best practices
- Creating reference materials
- Building knowledge base

**Output Format**: Word (.docx) or Markdown (.md)

**Typical Sections**:
1. Title and subtitle (Internal Reference Document)
2. Purpose
3. Overview
4. The Process (step-by-step)
5. Decision Points
6. Tools & Resources Needed
7. Common Issues & Solutions
8. Owner

**Example Request**:
```
"Create an internal process document for how to run a MAP session.
Include prep checklist, question flow, timing, and post-session deliverables.
Output as Markdown."
```

**What You'll Get**:
- Markdown document with clear structure
- "INTERNAL USE ONLY" marking
- Numbered process steps
- Decision trees for common scenarios
- Troubleshooting section
- Filename: `TNDS_Process_MapSession_[date].md`

---

### Standard Operating Procedures (SOPs)

**Purpose**: Establish repeatable, consistent processes

**When to Use**:
- Processes requiring compliance
- Quality-critical workflows
- Tasks multiple people execute
- Processes requiring audit trails
- Standardization across team

**Output Format**: Markdown (.md) preferred for version control

**Typical Sections**:
1. Title (SOP: Process Name)
2. Effective Date, Version, Status
3. Purpose
4. Scope (what's covered, what's not)
5. Roles & Responsibilities
6. Detailed Procedure
7. Quality Checks
8. Exceptions
9. Related Documents
10. Revision History

**Example Request**:
```
"Create an SOP for client onboarding after signed agreement.
Cover: payment confirmation, welcome email, kickoff scheduling, 
project setup, and handoff to delivery team."
```

**What You'll Get**:
- Structured SOP with all required sections
- Version number and effective date
- Clear roles and responsibilities
- Step-by-step procedure with timing
- Quality checklist
- Exception handling
- Revision history table
- Filename: `TNDS_SOP_ClientOnboarding_[date].md`

---

### Diagnostic Cheat Sheets

**Purpose**: Provide quick reference for assessments and calls

**When to Use**:
- Direction Protocol stages (IDENTIFY, ASSESS, MAP)
- Client qualification
- Discovery calls
- Technical diagnostics
- Quick reference during meetings

**Output Format**: Word document (.docx) for printability

**Typical Sections**:
1. Title and context
2. Before You Start (setup, opening script)
3. Question sections with timing
4. Red Flags / Green Flags
5. Scoring or decision matrix
6. Next steps and closing script

**Example Request**:
```
"Create a cheat sheet for the ASSESS stage.
30 minutes total, 5 sections: Operational Reality (10 min), 
Current State (8 min), Stakes (5 min), Fit Check (3 min), 
Budget Reality (2 min). Include red flags and green flags."
```

**What You'll Get**:
- Concise, printable reference guide
- Exact scripts to use
- Timed sections
- Clear red/green flag checklists
- Decision guidance
- Filename: `TNDS_Diagnostic_AssessStage_[date].docx`

---

### Proposals

**Purpose**: Present solution to client based on MAP session

**When to Use**:
- After completing MAP stage
- Presenting CHART to prospect
- Formal engagement proposals
- Complex multi-phase projects

**Output Format**: Word document (.docx)

**Typical Sections**:
1. Cover page
2. Executive summary
3. Current situation (from MAP)
4. Proposed solution
5. Scope & deliverables
6. Timeline and milestones
7. Investment & payment terms
8. Next steps

**Example Request**:
```
"Generate a proposal for Peak HVAC based on our MAP session.
12 techs, paper-based dispatch, need data-command, office-command, 
sms-command, financial-command. Price: $4,250. Timeline: 4 weeks."
```

**What You'll Get**:
- Professional, branded proposal
- Current state description
- Solution architecture
- Module breakdown
- Pricing justification
- Clear next steps
- Filename: `TNDS_Proposal_PeakHVAC_[date].docx`

---

### Technical Specifications

**Purpose**: Document technical architecture and implementation

**When to Use**:
- Planning implementation
- Developer handoffs
- System documentation
- API documentation
- Architecture decisions

**Output Format**: Markdown (.md) preferred

**Typical Sections**:
1. Overview
2. Technical requirements
3. System architecture
4. Data flows
5. Integrations
6. Security considerations
7. Testing approach
8. Deployment plan

**Example Request**:
```
"Create technical spec for financial-command module.
Needs: QuickBooks API integration, job costing calculations,
real-time P&L, Google Sheets sync. Use Markdown."
```

**What You'll Get**:
- Detailed technical documentation
- Architecture diagrams (ASCII)
- API specifications
- Data models
- Implementation steps
- Testing requirements
- Filename: `TNDS_Spec_FinancialCommand_[date].md`

---

## STEP-BY-STEP TUTORIALS

### Tutorial 1: Create Your First Service Document

**Goal**: Create a complete service document for Command Center Build

**Time**: 10-15 minutes

**Steps**:

**1. Initiate the request**
```
"Using the TNDS Documentation skill, create a service document 
for Command Center Build"
```

**2. Claude will confirm and may ask questions**
```
Claude: "I'll create a service document for Command Center Build. 
This is our core offering - $2,500-$5,000, 2-4 weeks. Should I use 
the standard template or are there customizations?"

You: "Standard template is fine"
```

**3. Review the generated document**

Claude will create a Word document with:
- TNDS logo centered in header
- Title: "Command Center Build"
- Subtitle in teal
- All sections filled with appropriate content
- Footer with contact information
- Navy and Teal colors throughout

**4. Request adjustments if needed**
```
You: "The 'Problems This Removes' section should focus more on 
financial visibility issues"

Claude: [Updates document and provides new link]
```

**5. Download and use**

Click the download link, save to your docs folder, ready to share with prospects.

**Success Criteria**:
- ✅ Document has TNDS branding
- ✅ All sections are complete
- ✅ Voice sounds like TNDS
- ✅ No corporate jargon
- ✅ Pricing and timeline accurate

---

### Tutorial 2: Create an Internal SOP

**Goal**: Document the client onboarding process

**Time**: 15-20 minutes

**Steps**:

**1. Gather information first**

Before creating the SOP, list out:
- Process steps
- Who's responsible for each step
- Timing/sequence
- Tools used
- Common issues

**2. Make the request**
```
"Create an SOP for client onboarding after signed agreement.

Process steps:
1. Confirm payment received (Sales Lead, within 24 hours)
2. Send welcome email (Sales Lead, same day)
3. Schedule kickoff meeting (Sales Lead, within 3 days)
4. Create project folder structure (Delivery Lead)
5. Set up project tracker entry (Delivery Lead)
6. Conduct kickoff meeting (Delivery Lead, within 5 days)

Common issues: 
- Payment delays
- Client not responding to scheduling
- Missing information for setup

Output as Markdown."
```

**3. Claude generates the SOP**

```
Claude: "I've created a complete SOP for Client Onboarding with:
- Purpose and scope clearly defined
- All 6 steps detailed with who/when/how
- Quality checks checklist
- Exception handling for common issues
- Revision history table

Saved as: TNDS_SOP_ClientOnboarding_2026-01-26.md
[Download link]"
```

**4. Review for accuracy**

Check:
- Are all steps correct?
- Are responsibilities assigned properly?
- Is timing realistic?
- Are quality checks comprehensive?

**5. Request refinements**
```
You: "Add a quality check for 'Client has access to shared workspace'"

Claude: [Updates SOP and provides new link]
```

**6. Implement**

- Add to your internal wiki
- Share with team
- Use for training
- Update version as process evolves

**Success Criteria**:
- ✅ All process steps documented
- ✅ Roles clearly assigned
- ✅ Quality checks included
- ✅ Exception handling covered
- ✅ Version controlled

---

### Tutorial 3: Create a Diagnostic Cheat Sheet

**Goal**: Build a reference tool for ASSESS stage calls

**Time**: 10 minutes

**Steps**:

**1. Define the structure**

Think through:
- Total time (30 minutes for ASSESS)
- Sections needed
- Questions for each section
- What signals to watch for

**2. Make a detailed request**
```
"Create a diagnostic cheat sheet for the ASSESS stage 
of Direction Protocol.

30 minutes total, structured as:

Section 1: Operational Reality (10 min)
- Walk me through your typical workflow
- Where do things usually go wrong?
- How do you find out when something's off?

Section 2: Current State (8 min)
- Where does your information live?
- How do you get visibility into [metrics]?
- Who else knows how things work?

Section 3: Stakes and Readiness (5 min)
- What's this costing you?
- Where are you in a year if nothing changes?
- What would be different if fixed?

Section 4: Fit Check (3 min)
- Explain MAP stage requirement
- Gauge openness

Section 5: Budget Reality (2 min)
- Budget range discussion

Red Flags:
- Won't commit to MAP
- Just wants price
- 'Tried everything' mentality

Green Flags:
- Specific pain examples
- Quantifies impact
- Decision maker engaged

Include opening and closing scripts."
```

**3. Claude generates the cheat sheet**

```
Claude: "I've created a complete ASSESS stage cheat sheet with:
- Opening script
- All 5 sections with exact questions and timing
- Red flag and green flag checklists
- Closing script and next steps
- Formatted for easy printing

Saved as: TNDS_Diagnostic_AssessStage_2026-01-26.docx
[Download link]"
```

**4. Print and test**

- Download and print
- Use on next ASSESS call
- Make notes on what works
- Refine based on experience

**5. Update as needed**
```
You: "Add a question about team size to Section 1"

Claude: [Updates and provides new version]
```

**Success Criteria**:
- ✅ Covers full 30-minute call
- ✅ Questions are clear and specific
- ✅ Timing helps pace the call
- ✅ Red/green flags actionable
- ✅ Scripts feel natural to use

---

### Tutorial 4: Generate a Client Proposal

**Goal**: Create a proposal for a prospect after MAP session

**Time**: 15-20 minutes

**Prerequisites**: Completed MAP session with detailed notes

**Steps**:

**1. Compile MAP session outputs**

Gather:
- Client name and details
- Current state description
- Pain points identified
- Proposed Command modules
- Pricing calculation
- Timeline estimate

**2. Make comprehensive request**
```
"Generate a proposal for Peak HVAC based on MAP session.

Client: Peak HVAC, Colorado Springs
Owner: Mike Thompson
Size: 12 technicians

Current State:
- Paper job tickets
- Whiteboard dispatch
- Text message coordination
- QuickBooks for invoicing
- 3-5 day lag from service to invoice
- Owner finds out about problems too late

Pain Points:
- No real-time visibility
- Lost/damaged paper tickets (10% of jobs)
- Delayed invoicing ($12-15K/year impact)
- Owner can't take day off

Proposed Solution:
- data-command (central data)
- office-command (dispatch automation)
- sms-command (tech notifications)
- financial-command (job costing + auto-invoicing)

Pricing: $4,250 (Base $3,500 + $750 field/office adjustment)
Timeline: 4 weeks
Payment: 40/30/30

Expected Outcomes:
- Real-time job status visibility
- Same-day invoicing
- Eliminate lost tickets
- Owner can delegate confidently
```

**3. Claude generates proposal**

```
Claude: "I've created a complete proposal for Peak HVAC including:
- Executive summary of their situation
- Visual representation of current vs desired state
- Detailed solution architecture
- Module breakdown with benefits
- Timeline with weekly milestones
- Investment breakdown and payment terms
- Expected ROI and outcomes
- Clear next steps

Saved as: TNDS_Proposal_PeakHVAC_2026-01-26.docx
[Download link]"
```

**4. Review for accuracy**

Verify:
- Client details correct
- Pricing matches MAP calculation
- Timeline realistic
- Modules address pain points
- Next steps clear

**5. Customize if needed**
```
You: "Add a section about the 30-day post-launch support included"

Claude: [Updates proposal]
```

**6. Present to client**

- Schedule CHART presentation
- Walk through proposal
- Handle objections
- Close or negotiate

**Success Criteria**:
- ✅ Accurately represents MAP findings
- ✅ Solution clearly addresses pain points
- ✅ Pricing justified and transparent
- ✅ Timeline believable
- ✅ Professional presentation quality

---

## BRAND GUIDELINES REFERENCE

### Voice & Tone

**The TNDS Voice Is**:
- Direct and clear
- Confident but not arrogant
- Military-influenced (precise, no-nonsense)
- Owner-to-owner (we get it)
- Outcomes-focused (not feature-focused)

**Writing Rules**:

**DO**:
- ✅ Use contractions (don't, won't, can't)
- ✅ Write in active voice
- ✅ Keep paragraphs short (2-4 sentences)
- ✅ Front-load important information
- ✅ Use specific examples
- ✅ Quantify when possible
- ✅ Address reader directly (you, your)

**DON'T**:
- ❌ Use emojis (NEVER)
- ❌ Use corporate buzzwords
- ❌ Write passive voice
- ❌ Apologize unnecessarily
- ❌ Hedge or qualify excessively
- ❌ Over-explain simple concepts

**Good vs Bad Examples**:

| Bad | Good |
|-----|------|
| Our cutting-edge solution leverages AI-powered automation to optimize workflows | You'll see every job in real-time and know when problems happen |
| We're passionate about helping you succeed | We fix operations that are broken |
| We offer transparent pricing models with clearly defined deliverables | Fixed scope, fixed price. No surprise invoices |
| Our team of experts will collaborate with stakeholders | We'll work with your team to build what you need |

---

### Visual Identity

**Logo Usage**:
- Always centered in document header
- Appropriate size (2-2.5 inches wide)
- Clear space around logo
- Never distort or recolor

**Color Palette**:

**Navy (Primary)** - #1a3a5c
- Use for: Main headers (H1, H3), body text, borders
- RGB: (26, 58, 92)

**Teal (Accent)** - #3d8eb9
- Use for: Secondary headers (H2), highlights, key phrases
- RGB: (61, 142, 185)

**Light Teal** - #5ba3c8
- Use for: Backgrounds, subtle emphasis
- RGB: (91, 163, 200)

**Supporting Colors**:
- Black: Body text
- Dark Gray (#404040): Quotes, secondary text
- White: Backgrounds, header text on teal

**Typography**:

**Font Family**: Arial (only)
- Never mix fonts
- Arial is clean, professional, widely available

**Font Sizes** (Word documents):
- H1 (Title): 36pt, Bold, Navy
- H2 (Major Section): 28pt, Bold, Teal
- H3 (Subsection): 24pt, Bold, Navy
- H4 (Minor Heading): 18pt, Bold, Navy
- Subtitle: 14pt, Italic, Teal
- Body Text: 11pt, Regular, Black
- Footer: 9pt, Regular, Navy

**Line Spacing**: 1.15 for body text

**Paragraph Spacing**:
- After paragraphs: 10pt
- After bullet points: 6pt
- After headers: Varies by level (12pt/10pt/8pt/6pt)

---

### Key Phrases

Use these consistently:

**The Transformation Statement**:
> "Direction Protocol gets you clarity. Command Protocol gets you control. That's how we turn data into direction."

**Use when**: Explaining the relationship between sales and delivery

**The Value Proposition**:
> "See what's happening in your operation so you can make better decisions and take a day off."

**Use when**: Describing what TNDS does

**The Pricing Philosophy**:
> "Fixed scope, fixed price. No open-ended projects. No surprise invoices."

**Use when**: Addressing cost or scope concerns

**Prerequisites Statement**:
> "Every engagement begins with the Direction Protocol: we Identify fit, Assess your situation, and Map your operation before we build anything."

**Use when**: Explaining the sales process

**Command Partner Selectivity**:
> "This is selective by design. Not every client gets offered this."

**Use when**: Describing premium/ongoing services

**Additional Phrases**:
- "We don't start with technology. We start with understanding your operation."
- "When we're done, you're in command of your operation instead of your operation commanding you."
- "Operations that existed before iPhones—businesses that need enterprise-grade automation without enterprise-grade complexity."

---

### The Two Protocols

**Direction Protocol (Sales)**:
The 5-stage process: IDENTIFY → ASSESS → MAP → CHART → LAUNCH

Always reference with:
- Correct stage names (capitalized)
- Correct timing (15-20 min, 30 min, 90-120 min, 30-45 min)
- Correct sequence (never skip stages)

**Command Protocol (Delivery)**:
Three service offerings:

**Command Center Build**
- Price: $2,500-$5,000
- Timeline: 2-4 weeks
- Deliverable: Operational visibility + Command modules

**Battle Rhythm Install**
- Price: $2,000-$4,000
- Timeline: 2-4 weeks
- Deliverable: Operating cadence + accountability

**Command Partner**
- Price: $1,000-$2,000/month
- Timeline: Ongoing
- Deliverable: Fractional ops support

**Command Modules**:
Always end in "-command" or "-ops":
- data-command, financial-command, analytics-command
- asset-command, office-command, onboard-command
- proposal-command, workspace-command, sms-command
- contract-command, realty-command, tax-command
- seo-command, govcon-command, compliance-gov-module

---

### ICP (Ideal Client Profile)

**Who We Work With**:
- 5-20 person operations
- Field service OR office operations
- Owner overwhelmed, no middle management
- Information scattered (texts, paper, spreadsheets)
- Decisions made blind
- Can't take a day off

**Who We Don't Work With**:
- Startups without ops foundation
- Anyone looking for "AI magic"
- Micromanagers who won't delegate
- No budget authority
- Won't commit to Direction Protocol
- Wrong size (too small or too big)

**Use ICP When**:
- Writing "Who This Is For" sections
- Creating qualification criteria
- Describing target audience
- Explaining fit

---

## TEMPLATE REFERENCE

### Client-Facing Service Document Template

```
[TITLE - Service Name]
[Subtitle - Who it's for or what it does (italicized, teal)]

## What This Engagement Is
[2-3 paragraphs explaining the service]
- What problem it solves
- How it works
- What makes it different

## Who This Is For
[Bullet list of ideal client characteristics]
- Use client language
- Paint a picture they see themselves in
- 5-10 bullets

## Problems This Removes
[Bullet list in first-person client voice]
- "I can't see what's happening..."
- "We always find out..."
- "Everything depends on..."

## What You Get

### [Component 1 Name]
- Specific deliverable
- What it does for them
- How they'll use it

### [Component 2 Name]
[Same structure]

## Scope & Pricing

**Investment**: $X,XXX (or range)
**Timeline**: X weeks
**Payment Terms**: 50/50 or 40/30/30

**What's Included**:
- [Specific inclusion]
- [Specific inclusion]

**What's Not Included**:
- [Specific exclusion]
- [Specific exclusion]

## Prerequisites
[What must be complete first]
- Every engagement begins with Direction Protocol
- [Other requirements]

## What Comes Next
[Optional - follow-on services]
- Next logical step
- How this positions them
```

---

### Internal Process Document Template

```
[Process Name]
[Internal Reference Document]

## Purpose
[Why this exists, when to use it, who should use it]

## Overview
[High-level summary, 2-3 paragraphs]
- Context
- Expected outcome
- Resources required

## The Process

### Step 1: [Action Name]
[What to do]
- Sub-step if needed
- Key considerations
- Tools required

[Continue for all steps]

## Decision Points

### When [Scenario X] Happens
**Do this**: [Action]
**Because**: [Reasoning]

## Tools & Resources Needed
- [Tool 1]: What it's for
- [Tool 2]: What it's for

## Common Issues & Solutions

**Issue**: [Problem]
**Solution**: [Fix]
**Prevention**: [How to avoid]

## Owner
**Maintained by**: [Name/Role]
**Last Updated**: [Date]
```

---

### SOP Template

```
# SOP: [Process Name]

**Effective Date**: [Date]
**Version**: [X.X]
**Status**: [Draft/Active/Archived]

## Purpose
[One sentence why this exists]

## Scope

**What This Covers**:
- [Included]
- [Included]

**What This Doesn't Cover**:
- [Excluded]
- [Excluded]

## Roles & Responsibilities

**[Role 1]**:
- [Responsibility]
- [Responsibility]

## Procedure

### 1. [Step Name]
**Action**: [What to do]
**Who**: [Role]
**When**: [Timing]
**How**: [Instructions]
**Output**: [Result]

[Continue for all steps]

## Quality Checks
- [ ] Check 1
- [ ] Check 2

## Exceptions
**When to Deviate**: [Conditions]
**How to Handle**: [Alternative]
**Who Approves**: [Authority]

## Related Documents
- [Document 1]
- [Document 2]

## Revision History
| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | [Date] | Initial | [Name] |
```

---

### Diagnostic Cheat Sheet Template

```
# [What This Is For]
[Duration or context]

## Before You Start

**Setup**:
- [Prep item]
- [Prep item]

**Opening Script**:
> "[Exact words]"

## Section 1: [Topic]
**Time**: [X minutes]

1. > "[Question]"
   - Listen for: [What to note]
   - Red flag: [Warning]
   - Green flag: [Good sign]

[Continue for all sections]

## Red Flags
- [ ] [Warning 1]
- [ ] [Warning 2]

**If 2+ red flags**: [Action]

## Green Flags
- [ ] [Positive 1]
- [ ] [Positive 2]

**If 3+ green flags**: [Action]

## Next Steps
**After this**:
1. [Action]
2. [Action]

**Closing Script**:
> "[Exact words]"
```

---

## ADVANCED FEATURES

### Creating Multiple Variations

**Scenario**: You need the same document in multiple formats

**Request**:
```
"Create a service document for Command Center Build in two formats:
1. Full Word document for client-facing use
2. Condensed Markdown version for internal wiki"
```

**Result**: Claude generates both versions, maintaining consistency

---

### Batch Document Generation

**Scenario**: You need documents for all three services

**Request**:
```
"Create service documents for all three Command Protocol offerings:
1. Command Center Build
2. Battle Rhythm Install
3. Command Partner

Use standard templates with appropriate pricing and details for each."
```

**Result**: Three complete, branded service documents

---

### Custom Sections

**Scenario**: You need a standard template with custom additions

**Request**:
```
"Create a service document for Command Center Build, 
but add a 'Case Studies' section before 'What Comes Next' 
with two brief client examples"
```

**Result**: Standard template plus your custom section

---

### Updating Existing Documents

**Scenario**: You have a document that needs refreshing

**Request**:
```
"I have an existing service document for Command Center Build.
Update it with:
- New pricing: $3,000-$6,000 (was $2,500-$5,000)
- Add asset-command to the modules list
- Update timeline to 3-5 weeks (was 2-4)
Keep everything else the same."
```

**Result**: Updated document with only specified changes

---

### Creating Document Families

**Scenario**: Related documents that reference each other

**Request**:
```
"Create a document family for Battle Rhythm Install:
1. Service document (client-facing)
2. Internal delivery checklist
3. SOP for implementation
4. Post-delivery handoff template

Make sure they reference each other appropriately."
```

**Result**: Four interlinked documents

---

### Language and Tone Variations

**Scenario**: Same content, different audiences

**Request**:
```
"Create two versions of the financial-command module doc:
1. Client-facing (simple language, outcome-focused)
2. Technical spec (detailed, architecture-focused)

Same module, different audiences."
```

**Result**: Two documents, same information, appropriate tone for each

---

## TROUBLESHOOTING

### Issue: Document doesn't have TNDS branding

**Symptoms**:
- No logo in header
- Wrong colors
- Generic formatting

**Cause**: Skill not loaded or referenced

**Solution**:
```
"Using the TNDS Documentation skill, [your request]"
```
Explicitly reference the skill name.

---

### Issue: Voice doesn't sound like TNDS

**Symptoms**:
- Corporate jargon present
- Passive voice
- Overly formal
- Apologetic tone

**Cause**: Not following voice guidelines

**Solution**: Request adjustment
```
"Make this sound more like TNDS - direct, no-fluff, 
outcomes-focused. Remove corporate jargon."
```

---

### Issue: Wrong template structure

**Symptoms**:
- Sections don't match expected template
- Missing required sections
- Incorrect order

**Cause**: Template not specified clearly

**Solution**: Be explicit
```
"Create a service document (client-facing template) for [X]"
```
or
```
"Create an SOP (standard operating procedure template) for [X]"
```

---

### Issue: Information is incorrect

**Symptoms**:
- Wrong pricing
- Incorrect timeline
- Outdated modules

**Cause**: Skill has outdated information OR you need to provide specifics

**Solution**: Provide current details
```
"Create service doc for Command Center Build.
Current pricing: $2,500-$5,000
Current timeline: 2-4 weeks
Current modules: data-command, financial-command, analytics-command, 
office-command, asset-command"
```

---

### Issue: Logo not appearing

**Symptoms**:
- Header has text but no logo image
- Placeholder text instead of logo

**Cause**: Logo file not accessible

**Solution**: 
1. Verify logo file exists: `/mnt/user-data/uploads/word-doc-tnds-logo.png`
2. If using Claude Desktop, ensure logo is in skill directory
3. Request fallback: "Use text header if logo unavailable"

---

### Issue: Document too generic

**Symptoms**:
- Content feels boilerplate
- Doesn't address specific use case
- Missing key details

**Cause**: Not enough context provided

**Solution**: Provide detailed information
```
Instead of: "Create service doc for Command Center Build"

Use: "Create service doc for Command Center Build targeting 
HVAC companies with 8-15 techs who use paper tickets and have 
no real-time visibility. Emphasize the dispatch automation and 
same-day invoicing benefits."
```

---

### Issue: Formatting inconsistent

**Symptoms**:
- Spacing varies
- Font sizes wrong
- Colors don't match brand

**Cause**: Document generation issue

**Solution**: Request regeneration
```
"Regenerate with strict adherence to TNDS formatting specs:
- Navy H1 at 36pt
- Teal H2 at 28pt
- 11pt body
- 1.15 line spacing
- Logo centered in header"
```

---

## BEST PRACTICES

### Before Creating Any Document

**1. Know Your Audience**
- Client-facing? Use Word, full branding
- Internal team? Word or Markdown
- Technical? Markdown preferred

**2. Gather Information**
- What's the purpose?
- What sections are needed?
- What specific details matter?
- What's the call to action?

**3. Choose the Right Template**
- Service doc for offerings
- SOP for processes
- Cheat sheet for quick reference
- Process doc for workflows

**4. Provide Context**
- Don't rely on Claude to guess
- Specify pricing, timing, details
- Reference Direction/Command Protocol correctly

---

### While Creating

**1. Be Specific in Requests**

Poor:
```
"Create a document about our services"
```

Good:
```
"Create a client-facing service document for Command Center Build.
Price: $2,500-$5,000, Timeline: 2-4 weeks. Target: 5-20 person 
operations with scattered data and no real-time visibility."
```

**2. Iterate and Refine**
- First draft is rarely perfect
- Request specific changes
- Refine until it's right

**3. Check Against Brand**
- Does it sound like TNDS?
- Is branding correct?
- Are key phrases used?

---

### After Creating

**1. Quality Check**

Use this checklist:

**Content**:
- [ ] Voice matches TNDS tone
- [ ] No corporate jargon
- [ ] Outcomes-focused language
- [ ] Specific and concrete
- [ ] No emojis

**Branding**:
- [ ] Logo in header (Word docs)
- [ ] Navy and Teal colors correct
- [ ] Arial font throughout
- [ ] Footer with contact info
- [ ] Proper spacing

**Accuracy**:
- [ ] Pricing current
- [ ] Timeline realistic
- [ ] Contact info correct
- [ ] Links work (if any)

**Completeness**:
- [ ] All sections present
- [ ] No [TODO] or [TBD] markers
- [ ] Clear next steps

**2. Save and Organize**

**File Naming**: `TNDS_[Type]_[Name]_[Date].ext`

**Storage**:
- Client-facing: Sales folder
- Internal: Team wiki or Notion
- SOPs: Procedures directory
- Technical: Developer docs

**Version Control**:
- Markdown: Use Git
- Word: Document version in filename
- Track major changes

**3. Share Appropriately**

**Client-Facing**:
- Review before sharing
- Send as PDF for final version
- Follow up after they review

**Internal**:
- Add to wiki/knowledge base
- Announce to team
- Gather feedback

**Technical**:
- Commit to repository
- Link from related docs
- Keep updated

---

### Maintaining Consistency

**1. Use Templates Consistently**
- Same template for same document type
- Don't mix and match structures

**2. Update Centrally**
- When pricing changes, update skill
- When services change, update templates
- Keep one source of truth

**3. Train Team**
- Share this manual
- Review examples together
- Establish review process

**4. Periodic Review**
- Quarterly: Review all client-facing docs
- Monthly: Review internal docs
- As needed: Update SOPs

---

## FAQ

### General Questions

**Q: Can I create documents without explicitly referencing the skill?**

A: It's best to reference it explicitly: "Using the TNDS Documentation skill..." This ensures Claude loads the correct guidelines.

**Q: What if I need a document type not in the templates?**

A: Describe what you need and reference the closest template. For example: "Create a document similar to the service doc template, but for a training program."

**Q: Can I modify the brand colors or fonts?**

A: Not recommended. Consistency is key to brand identity. If you absolutely must, be explicit: "Use the standard template but with [specific change]."

**Q: How do I update the skill when services or pricing change?**

A: Edit the SKILL.md file, update the relevant sections, increment the version number, and test with a sample document.

---

### Document Creation

**Q: How long does it take to create a document?**

A: 
- Simple service doc: 2-5 minutes
- Complex SOP: 5-10 minutes
- Technical spec: 10-15 minutes
- Full proposal: 15-20 minutes

**Q: Can I create documents in other languages?**

A: The skill is optimized for English. For other languages, request: "Create in [language] while maintaining TNDS voice and branding."

**Q: What if the document is too long?**

A: Request conciseness: "Make this more concise - max 3 pages" or "Reduce the 'What This Is' section to 2 paragraphs."

**Q: What if the document is too short?**

A: Request expansion: "Expand the 'What You Get' section with more detail about each module" or "Add examples to each problem statement."

---

### Formatting

**Q: Why Word for client-facing and Markdown for internal?**

A: 
- Word: Professional, printable, full branding, clients expect it
- Markdown: Easy to edit, version control friendly, portable, technical team prefers it

**Q: Can I get both Word and Markdown versions?**

A: Yes! Request: "Create in both Word and Markdown formats."

**Q: How do I adjust spacing or fonts?**

A: Request: "Increase spacing after headers" or "Use 12pt body text instead of 11pt." But be careful - deviation from brand specs reduces consistency.

**Q: Can I add images or diagrams?**

A: Yes, but you'll need to insert them manually after generation. Request placeholders: "Add a [DIAGRAM: workflow] placeholder where the process diagram should go."

---

### Content

**Q: How do I make the voice more/less formal?**

A: 
- More direct: "Make this more direct and concise"
- More detailed: "Add more explanation for non-technical audiences"
- More casual: "Make this feel more conversational"

Note: TNDS voice is already fairly direct. Going too casual breaks brand.

**Q: What if I don't have all the information?**

A: 
1. Provide what you have
2. Request placeholders: "Use [TBD] for pricing since we haven't calculated it yet"
3. Fill in later

**Q: Can I use client-specific examples?**

A: Absolutely! "In the 'Problems This Removes' section, use these specific examples from Peak HVAC: [examples]."

---

### Technical

**Q: Where are documents saved?**

A: `/mnt/user-data/outputs/` directory. Claude provides download links.

**Q: What if the logo doesn't appear?**

A: Verify the logo file path. Default: `/mnt/user-data/uploads/word-doc-tnds-logo.png`. If unavailable, Claude uses text fallback.

**Q: Can I edit the generated Word document?**

A: Yes! Download it and edit in Microsoft Word or Google Docs. The formatting is standard and editable.

**Q: How do I version control Word documents?**

A: 
- Include date in filename
- Use "track changes" for edits
- Or convert to Markdown for Git versioning

---

### Collaboration

**Q: Can multiple people use this skill?**

A: Yes! Share the skill files with your team. Everyone gets consistent output.

**Q: How do I share templates with team members?**

A: 
1. Give them access to this manual
2. Share the skill files
3. Show examples from examples.md
4. Have them practice with simple docs first

**Q: What if team members create off-brand documents?**

A: 
- Use this manual for training
- Implement review process
- Share good examples
- Provide feedback on deviations

---

### Updates and Maintenance

**Q: How often should I update the skill?**

A: 
- When services change
- When pricing updates
- When processes evolve
- Quarterly review minimum

**Q: How do I keep old documents current?**

A: 
- Track document versions
- Schedule periodic reviews
- Update high-visibility docs first
- Deprecate outdated materials

**Q: What if TNDS branding changes?**

A: 
1. Update SKILL.md with new guidelines
2. Regenerate key documents
3. Update logo file
4. Test with sample documents

---

## APPENDIX

### A. Complete Brand Color Reference

| Color | Hex Code | RGB | When to Use |
|-------|----------|-----|-------------|
| Navy (Primary) | #1a3a5c | (26, 58, 92) | H1, H3, body text, borders |
| Teal (Accent) | #3d8eb9 | (61, 142, 185) | H2, highlights, key phrases |
| Light Teal | #5ba3c8 | (91, 163, 200) | Backgrounds, subtle emphasis |
| Black | #000000 | (0, 0, 0) | Body text |
| Dark Gray | #404040 | (64, 64, 64) | Quotes, secondary text |
| White | #ffffff | (255, 255, 255) | Backgrounds, reverse text |

---

### B. Typography Scale

| Element | Size | Weight | Color | Usage |
|---------|------|--------|-------|-------|
| H1 | 36pt | Bold | Navy | Document title |
| H2 | 28pt | Bold | Teal | Major sections |
| H3 | 24pt | Bold | Navy | Subsections |
| H4 | 18pt | Bold | Navy | Minor headings |
| Subtitle | 14pt | Italic | Teal | Document subtitle |
| Body | 11pt | Regular | Black | Body text |
| Quote | 10pt | Italic | Dark Gray | Quoted text |
| Footer | 9pt | Regular | Navy | Footer text |

---

### C. Document Type Quick Reference

| Need | Document Type | Template | Format |
|------|--------------|----------|--------|
| Describe a service | Service Document | Client-Facing Service | Word |
| Create a proposal | Proposal | Proposal | Word |
| Document a process | Process Doc | Internal Process | Word/MD |
| Standardize a procedure | SOP | SOP | Markdown |
| Create call guide | Cheat Sheet | Diagnostic | Word |
| Technical docs | Tech Spec | Technical Spec | Markdown |
| Service contract | Agreement | Agreement | Word |

---

### D. Common Request Patterns

**Pattern 1: Simple Service Doc**
```
"Create a service document for [service name]"
```

**Pattern 2: Detailed Service Doc**
```
"Create a service document for [service name].
Price: [price]
Timeline: [timeline]
Target audience: [description]
Key benefits: [benefits]"
```

**Pattern 3: Internal SOP**
```
"Create an SOP for [process name].
Steps: [list of steps]
Roles: [who does what]
Tools: [what's needed]
Output as Markdown."
```

**Pattern 4: Diagnostic Tool**
```
"Create a cheat sheet for [stage/process].
Duration: [time]
Sections: [list sections with timing]
Include: [red flags, green flags, scripts]"
```

**Pattern 5: Technical Spec**
```
"Create technical spec for [module/feature].
Requirements: [list]
Integrations: [list]
Architecture: [description]
Output as Markdown."
```

**Pattern 6: Client Proposal**
```
"Generate proposal for [client] based on MAP session.
Current state: [description]
Proposed solution: [modules]
Pricing: [amount]
Timeline: [weeks]"
```

---

### E. Skill File Locations

**Standard Installation**:
```
tnds-documentation-skill/
├── SKILL.md (Main skill)
├── README.md (Overview)
├── document-tools.md (Python utilities)
├── examples.md (Example outputs)
├── USER-MANUAL.md (This document)
└── word-doc-tnds-logo.png (Logo file)
```

**Logo Path Options**:
- `/mnt/user-data/uploads/word-doc-tnds-logo.png` (uploaded files)
- `./word-doc-tnds-logo.png` (skill directory)

**Output Location**:
- `/mnt/user-data/outputs/` (generated documents)

---

### F. Version History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | 2026-01-26 | Initial release of User Manual | Jacob Johnston |

---

### G. Glossary

**Brand Guidelines**: Visual and verbal standards for TNDS identity  
**Command Module**: Technical building block ending in "-command" or "-ops"  
**Command Protocol**: The delivery methodology (what we build)  
**Direction Protocol**: The sales methodology (how we qualify and scope)  
**ICP**: Ideal Client Profile - who we work best with  
**MAP Stage**: 90-120 minute diagnostic session in Direction Protocol  
**SOP**: Standard Operating Procedure  
**Template**: Predefined document structure  
**Voice**: The consistent personality and tone of TNDS writing

---

### H. Contact and Support

**Primary Contact**:  
Jacob Johnston  
719-204-6365  
jacob@truenorthstrategyops.com

**Company**:  
True North Data Strategies  
Colorado Springs, CO  
VOSB/SDVOSB Certified

**For Skill Issues**:
- Review this manual
- Check examples.md
- Consult SKILL.md
- Contact Jacob

**For Brand Questions**:
- Reference brand guidelines section
- Review voice examples
- Check existing documents
- Contact Jacob

---

## QUICK START CHECKLIST

For new users, complete these steps:

### Day 1: Orientation
- [ ] Read Introduction and Getting Started sections
- [ ] Verify skill installation
- [ ] Create a test document
- [ ] Review brand guidelines

### Day 2: Practice
- [ ] Complete Tutorial 1 (Service Document)
- [ ] Review voice & tone guidelines
- [ ] Study key phrases
- [ ] Create a simple internal doc

### Day 3: Application
- [ ] Complete Tutorial 2 (SOP)
- [ ] Create a real document you need
- [ ] Review quality checklist
- [ ] Share with team for feedback

### Week 1: Mastery
- [ ] Create all common document types
- [ ] Practice refining and iterating
- [ ] Build your template library
- [ ] Train others if applicable

---

**END OF USER MANUAL**

---

**True North Data Strategies**
Turning Data into Direction

Jacob Johnston | 719-204-6365 | jacob@truenorthstrategyops.com
Colorado Springs, CO • VOSB/SDVOSB

---

## Legal

**Confidentiality Notice:** This document contains proprietary methodology and trade secrets of True North Data Strategies LLC. Unauthorized reproduction, distribution, or disclosure is prohibited.

**Trademarks:** Direction Protocol™, Command Protocol™, Bearing Check™, World Model Mapper™, ARO Assessment™, Battle Rhythm Install™, and Command Center Build™ are trademarks of True North Data Strategies LLC.

---

© 2026 True North Data Strategies LLC. All rights reserved.
