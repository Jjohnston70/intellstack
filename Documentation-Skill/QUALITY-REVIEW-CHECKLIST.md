# Documentation Quality Review Checklist

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Ensure consistent quality standards for all TNDS documentation

---

## Overview

This checklist ensures every TNDS document meets quality standards before delivery. Use it:
1. **During creation** — Check as you write
2. **Before finalizing** — Complete review before saving
3. **Before delivery** — Final verification before sending

---

## Part 1: Pre-Creation Checklist

Before starting any document, verify:

### Request Clarity
- [ ] Audience is identified (client, team, technical)
- [ ] Purpose is clear (what action should reader take?)
- [ ] Format is decided (Word or Markdown)
- [ ] Timeline is understood
- [ ] Source skill identified (Direction Protocol, Command Protocol, etc.)

### Template Selection
- [ ] Correct template selected for document type
- [ ] Template structure reviewed before starting
- [ ] Any modifications to template noted

### Information Gathering
- [ ] All required information is available
- [ ] Source documents/outputs are accessible
- [ ] Subject matter expert consulted (if needed)
- [ ] Missing information gaps identified

**Pre-Creation Gate:**
All boxes must be checked before proceeding to content development.

---

## Part 2: Content Quality Checklist

### Voice & Tone

**Must Pass All:**
- [ ] Direct, no-fluff communication (no marketing speak)
- [ ] Active voice used (not passive)
- [ ] Confident tone (no hedging: "we try to...", "we hope to...")
- [ ] Outcomes-focused ("you'll be able to..." not "this does...")
- [ ] No emojis anywhere
- [ ] No corporate buzzwords (synergy, leverage, ecosystem)
- [ ] No jargon without definition
- [ ] Short paragraphs (2-4 sentences)

**Voice Check Questions:**

| Question | Good Answer |
|----------|-------------|
| Would I say this to a business owner over coffee? | Yes |
| Does this sound like marketing copy? | No |
| Could this be shorter? | No |
| Is any sentence over 25 words? | No |

---

### Language Patterns

**Correct Usage:**

| Wrong | Right |
|-------|-------|
| "Our solution leverages..." | "You'll see..." |
| "We strive to provide..." | "You get..." |
| "Stakeholder alignment" | "Everyone on the same page" |
| "Optimize operational workflows" | "Fix how work gets done" |
| "Enterprise-grade" | "Built for serious operations" |
| "We hope to..." | "We will..." |

**Key Phrase Usage:**
- [ ] Transformation statement used appropriately (if applicable)
- [ ] Value proposition stated clearly
- [ ] Pricing philosophy reflected (fixed scope, fixed price)
- [ ] Prerequisites statement included (if applicable)

---

### Content Specificity

- [ ] Specific examples used (not vague generalities)
- [ ] Numbers and quantifications included where possible
- [ ] Deliverables are concrete and measurable
- [ ] Timeline is realistic and specific
- [ ] Pricing is accurate (if applicable)

**Specificity Test:**

| Vague (Fix) | Specific (Good) |
|-------------|-----------------|
| "Improve efficiency" | "Cut invoice time from 3 days to same-day" |
| "Better visibility" | "See every job status in real-time" |
| "Enhanced communication" | "Automatic text alerts when technicians arrive" |
| "Ongoing support" | "Weekly 30-minute check-in calls" |

---

### Audience Appropriateness

**For Client Documents:**
- [ ] Language is non-technical (plain English)
- [ ] Benefits emphasized over features
- [ ] Client perspective used ("you" language)
- [ ] No internal jargon or abbreviations

**For Internal Documents:**
- [ ] Appropriate technical detail level
- [ ] Action-oriented instructions
- [ ] Clear ownership and responsibilities
- [ ] Internal abbreviations defined on first use

**For Technical Documents:**
- [ ] Technical accuracy verified
- [ ] Implementation details complete
- [ ] Code/config examples included where helpful
- [ ] Assumptions documented

---

## Part 3: Structure Quality Checklist

### Organization

- [ ] Follows appropriate template structure
- [ ] Logical flow from section to section
- [ ] Most important information appears first
- [ ] Related information grouped together
- [ ] Clear progression (setup → action → outcome)

### Headers & Hierarchy

- [ ] Headers create clear hierarchy (H1 → H2 → H3)
- [ ] Headers are descriptive (not generic like "Section 1")
- [ ] No skipped header levels (H1 → H3)
- [ ] Headers match document purpose

### Lists & Formatting

- [ ] Bullets used for 2+ unordered items
- [ ] Numbers used for sequential steps
- [ ] Single items written as prose (not bullets)
- [ ] List items parallel in structure
- [ ] Tables used where they improve clarity

### Section Length

- [ ] No section longer than one page without subsections
- [ ] Paragraphs are 2-4 sentences
- [ ] Bullet lists have 3-7 items (break up longer lists)
- [ ] Introduction and conclusion are concise

---

## Part 4: Brand Quality Checklist

### For Word Documents (.docx)

#### Header
- [ ] TNDS logo present
- [ ] Logo centered
- [ ] Logo height: ~0.8-1.0 inches
- [ ] Space after logo: ~0.2 inches

#### Typography
- [ ] H1: Arial, 36pt, Bold, Navy (#1a3a5c)
- [ ] H2: Arial, 28pt, Bold, Teal (#3d8eb9)
- [ ] H3: Arial, 24pt, Bold, Navy (#1a3a5c)
- [ ] H4: Arial, 18pt, Bold, Navy (#1a3a5c)
- [ ] Body: Arial, 11pt, Regular, Black
- [ ] No other fonts used

#### Colors
- [ ] Navy (#1a3a5c) used for primary headers
- [ ] Teal (#3d8eb9) used for secondary headers
- [ ] Black used for body text
- [ ] No random colors
- [ ] Light teal (#5ba3c8) for backgrounds only (20% opacity)

#### Spacing
- [ ] After H1: 12pt
- [ ] After H2: 10pt
- [ ] After H3: 8pt
- [ ] After paragraphs: 10pt
- [ ] After bullet points: 6pt
- [ ] Line spacing: 1.15

#### Footer
- [ ] Line 1: Jacob Johnston | 719-204-6365 | jacob@truenorthstrategyops.com
- [ ] Line 2: True North Data Strategies • Colorado Springs, CO (italicized)
- [ ] Font: Arial, 9pt
- [ ] Alignment: Centered
- [ ] Color: Navy (#1a3a5c)

#### Page Layout
- [ ] Margins: 1" all sides
- [ ] Page size: US Letter (8.5" x 11")
- [ ] Orientation: Portrait (unless content requires landscape)
- [ ] No widows/orphans (single lines at top/bottom of page)
- [ ] Page breaks in logical places

---

### For Markdown Documents (.md)

#### Structure
- [ ] Proper header hierarchy (#, ##, ###)
- [ ] Single # for document title only
- [ ] Consistent header formatting

#### Lists
- [ ] Bullets: `-` or `*` (consistent)
- [ ] Sub-items: 2-space indent
- [ ] Numbered lists: 3-space indent for sub-items

#### Special Formatting
- [ ] Blockquotes (`>`) for scripts/exact words
- [ ] Code blocks (```) for code or config
- [ ] Bold (`**`) for emphasis
- [ ] Tables formatted with pipes and dashes

#### Frontmatter (if used)
- [ ] Valid YAML syntax
- [ ] Title, author, date included
- [ ] Type specified

---

## Part 5: Template-Specific Checklists

### Client-Facing Service Document

**Required Sections:**
- [ ] Document title and subtitle
- [ ] What This Engagement Is (2-3 paragraphs)
- [ ] Who This Is For (bullet list)
- [ ] Problems This Removes (client voice)
- [ ] What You Get (deliverables)
- [ ] Scope & Pricing (investment, timeline, payment)
- [ ] Prerequisites (if applicable)
- [ ] What Comes Next (optional)

**Quality Points:**
- [ ] Pain points in first-person client language
- [ ] Deliverables specific and concrete
- [ ] Pricing clear (no ranges unless necessary)
- [ ] Prerequisites reference Direction Protocol

---

### Proposal

**Required Sections:**
- [ ] Cover page (logo, title, client name, date)
- [ ] Executive summary (1 page max)
- [ ] Current situation (from MAP)
- [ ] Proposed solution
- [ ] Scope & deliverables
- [ ] Timeline
- [ ] Investment & payment terms
- [ ] Next steps

**Quality Points:**
- [ ] Client name spelled correctly
- [ ] MAP findings accurately reflected
- [ ] Scope boundaries clear (what's in/out)
- [ ] Timeline realistic
- [ ] Payment terms specific

---

### Agreement

**Required Sections:**
- [ ] Parties (names, addresses)
- [ ] Services description
- [ ] Scope of work
- [ ] Timeline & milestones
- [ ] Payment terms
- [ ] Deliverables
- [ ] Client responsibilities
- [ ] Change orders
- [ ] Termination
- [ ] Signatures

**Quality Points:**
- [ ] Legal review recommended note included
- [ ] Dates and amounts verified
- [ ] Client responsibilities clearly stated
- [ ] Change order process defined

---

### SOP

**Required Sections:**
- [ ] SOP header (effective date, version, status)
- [ ] Purpose (one sentence)
- [ ] Scope (what's covered, what's not)
- [ ] Roles & responsibilities
- [ ] Procedure (step-by-step)
- [ ] Quality checks
- [ ] Exceptions
- [ ] Related documents
- [ ] Revision history

**Quality Points:**
- [ ] Each step has Who, What, When, How
- [ ] Quality checks are actionable
- [ ] Exception handling clear
- [ ] Version tracking in place

---

### Diagnostic/Cheat Sheet

**Required Sections:**
- [ ] Title and duration/context
- [ ] Before You Start (setup)
- [ ] Opening script (exact words)
- [ ] Sections with timed questions
- [ ] Red flags / Green flags
- [ ] Next steps
- [ ] Closing script (exact words)

**Quality Points:**
- [ ] Scripts are exact words (not paraphrased)
- [ ] Timing realistic for each section
- [ ] Red flags clearly defined
- [ ] Action for flag count specified

---

## Part 6: Pre-Delivery Checklist

### Final Review

- [ ] Read document aloud (catches awkward phrasing)
- [ ] Spell check completed
- [ ] Grammar check completed
- [ ] All placeholders filled in (no [brackets] remaining)
- [ ] Contact information correct
- [ ] Dates accurate
- [ ] Pricing verified (if applicable)

### File Naming

**Convention:** `TNDS_[Type]_[Name]_[Date].ext`

- [ ] Follows naming convention
- [ ] Type code correct
- [ ] Name is descriptive
- [ ] Date format: YYYY-MM-DD
- [ ] Extension correct (.docx or .md)

**Type Codes:**
| Code | Document Type |
|------|---------------|
| Service | Client-facing service doc |
| Proposal | Client proposal |
| Agreement | Contract |
| SOP | Standard operating procedure |
| Process | Internal process doc |
| Diagnostic | Cheat sheet/assessment |
| Spec | Technical specification |
| Training | Training materials |
| Module | Module documentation |

---

### Accessibility Check (for client documents)

- [ ] Font size readable (11pt minimum for body)
- [ ] Sufficient color contrast
- [ ] Headers used for structure (not just bold text)
- [ ] Tables have header rows
- [ ] Links are descriptive (not "click here")

---

### Save Location

- [ ] Saved to correct folder
- [ ] Previous version archived (if revision)
- [ ] Backup created (for critical documents)

---

## Part 7: Common Quality Issues

### Issue 1: Vague Language

**Symptom:** Document uses generic descriptions without specifics.

**Examples:**
| Vague | Fix |
|-------|-----|
| "Improve operations" | "Cut response time from 4 hours to 30 minutes" |
| "Better visibility" | "See every technician's location in real-time" |
| "Streamline processes" | "Eliminate 3 hours of weekly data entry" |

**Fix:** Add numbers, examples, or specific outcomes.

---

### Issue 2: Wrong Voice

**Symptom:** Document sounds like marketing copy or corporate memo.

**Examples:**
| Wrong Voice | Fix |
|-------------|-----|
| "We leverage cutting-edge technology..." | "You'll see everything in one place..." |
| "Our innovative solution enables..." | "This shows you..." |
| "Stakeholders will benefit from..." | "Your team will be able to..." |

**Fix:** Rewrite in plain, direct language. Read aloud to test.

---

### Issue 3: Missing Outcomes

**Symptom:** Document lists features without explaining benefits.

**Examples:**
| Feature Only | With Outcome |
|--------------|--------------|
| "Includes dashboard" | "Dashboard shows every job so you know when problems happen" |
| "Automated notifications" | "Automatic texts tell customers when you're on the way" |
| "Data integration" | "No more copying data between systems" |

**Fix:** For every feature, add "so that..." or "which means..."

---

### Issue 4: Inconsistent Formatting

**Symptom:** Fonts, colors, or spacing vary throughout document.

**Fix:**
1. Check brand specifications in SKILL.md
2. Apply consistent styles to all similar elements
3. Use style templates if available

---

### Issue 5: Missing Information

**Symptom:** Document has gaps or placeholder text.

**Examples:**
- "[Insert pricing here]"
- "Timeline: TBD"
- "Contact: [Name]"

**Fix:** Never deliver documents with placeholders. Get the information or note it's pending.

---

### Issue 6: Too Long

**Symptom:** Document has unnecessary sections or repetition.

**Fix:**
1. Cut any section that doesn't serve the reader
2. Combine repetitive content
3. Use tables instead of prose for comparisons
4. Ask: "Would cutting this hurt the document?"

---

## Part 8: Quality Metrics

### Track These Metrics

| Metric | Target | How to Measure |
|--------|--------|----------------|
| Revision request rate | <10% | # revisions / # documents |
| Checklist completion | 100% | Checklists fully completed |
| Time to delivery | On schedule | Actual vs. promised |
| Client acceptance | >95% | Proposals accepted without major revision |

---

## Quick Quality Check (5 minutes)

For time-pressured reviews, verify at minimum:

1. [ ] Voice is direct and outcomes-focused
2. [ ] No placeholders or missing information
3. [ ] Logo and footer are correct
4. [ ] File named correctly
5. [ ] Saved to correct location

**If any fail:** Stop and fix before delivery.

---

## Quality Review Process

### Self-Review (Required)

Complete full checklist before considering document "done."

### Peer Review (Recommended for)

- Client proposals over $5,000
- Service agreements
- Client-facing documents for new clients
- Documents in unfamiliar domains

### Subject Matter Expert Review (Required for)

- Technical specifications
- Legal agreements (legal review)
- Pricing documents (owner approval)

---

**Document Status:** Active
**Next Review:** After 20 documents reviewed using this checklist
**Feedback:** Track which issues occur most frequently

