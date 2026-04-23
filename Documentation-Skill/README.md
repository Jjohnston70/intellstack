# TNDS Documentation Skill

## Overview

The TNDS Documentation skill creates professionally branded documents following True North Data Strategies' established voice, structure, and visual identity. This ensures consistency across all client-facing materials, internal processes, SOPs, and technical documentation.

**Key Capabilities**:
- Generate Word documents (.docx) with full TNDS branding
- Create Markdown documents (.md) for technical/internal use
- Apply consistent voice and tone across all content
- Use standardized templates for different document types
- Maintain brand colors, typography, and formatting

---

## Quick Start

### Simple Usage

Just tell Claude what type of document you need:

```
"Create a service document for Command Center Build"
→ Generates client-facing service doc with full branding

"Create an SOP for client onboarding"
→ Generates standard operating procedure

"Create a cheat sheet for the ASSESS stage"
→ Generates diagnostic tool for sales calls
```

Claude will:
1. Select the appropriate template
2. Apply TNDS branding and formatting
3. Generate content following voice guidelines
4. Save to `/mnt/user-data/outputs/`
5. Provide download link

---

## What This Skill Does

### Document Types Supported

**Client-Facing Documents** (Word):
- Service descriptions
- Proposals
- Service agreements
- Professional presentations
- Engagement overviews

**Internal Documents** (Word or Markdown):
- Process documentation
- Standard Operating Procedures (SOPs)
- Team training materials
- How-to guides
- Diagnostic cheat sheets

**Technical Documents** (Markdown):
- Technical specifications
- System architecture docs
- API documentation
- Implementation guides
- Developer references

### Branding Applied

**Visual Identity**:
- TNDS logo in header (centered)
- Brand colors: Navy (#1a3a5c), Teal (#3d8eb9)
- Arial typography throughout
- Professional footer with contact info
- Consistent spacing and formatting

**Voice & Tone**:
- Direct, no-fluff communication
- Military-influenced clarity
- Confident but not arrogant
- Outcomes over features
- Owner-to-owner language

---

## File Structure

```
Documentation-Skill/
│
├── SKILL.md                           # Main skill definition
├── USER-MANUAL.md                     # Usage guide
├── README.md                          # This file
├── word-doc-tnds-logo.png            # TNDS logo for headers
│
├── WORKFLOW.md                        # Step-by-step document creation process
├── SKILL-INTEGRATIONS.md             # Integration with other TNDS skills
├── QUALITY-REVIEW-CHECKLIST.md       # Quality standards checklist
│
├── TRAINING-GUIDE.md                  # Onboarding guide for new users
├── CASE-STUDIES.md                    # Real-world document creation examples
├── EMAIL-TEMPLATES.md                 # Email templates for document delivery
│
├── PROPOSAL-TEMPLATE.md              # Detailed proposal creation guide
├── AGREEMENT-TEMPLATE.md             # Service agreement guide
├── MODULE-DOCUMENTATION-TEMPLATE.md   # Module documentation templates
│
├── FOLDER-STRUCTURE.md               # File organization standards
├── METRICS-DASHBOARD.md              # Quality and output tracking
│
├── document-tools.md                  # Python utilities for generation
├── examples.md                        # Example outputs
├── documentation-gaps.md             # Gap analysis
└── todo.md                           # Implementation tracking
```

---

## Document Navigation

### I want to...

| Goal | Go To |
|------|-------|
| Understand the documentation skill | [SKILL.md](SKILL.md) |
| Create a document step-by-step | [WORKFLOW.md](WORKFLOW.md) |
| Check document quality | [QUALITY-REVIEW-CHECKLIST.md](QUALITY-REVIEW-CHECKLIST.md) |
| See real examples | [CASE-STUDIES.md](CASE-STUDIES.md) |
| Learn the skill | [TRAINING-GUIDE.md](TRAINING-GUIDE.md) |
| Create a proposal | [PROPOSAL-TEMPLATE.md](PROPOSAL-TEMPLATE.md) |
| Create an agreement | [AGREEMENT-TEMPLATE.md](AGREEMENT-TEMPLATE.md) |
| Document a module | [MODULE-DOCUMENTATION-TEMPLATE.md](MODULE-DOCUMENTATION-TEMPLATE.md) |
| Send document emails | [EMAIL-TEMPLATES.md](EMAIL-TEMPLATES.md) |
| Understand skill integrations | [SKILL-INTEGRATIONS.md](SKILL-INTEGRATIONS.md) |
| Organize files correctly | [FOLDER-STRUCTURE.md](FOLDER-STRUCTURE.md) |
| Track documentation metrics | [METRICS-DASHBOARD.md](METRICS-DASHBOARD.md) |

---

## Brand Guidelines

### Company Information
- **Company**: True North Data Strategies
- **Tagline**: Turning Data into Direction
- **Owner**: Jacob Johnston
- **Contact**: 719-204-6365 | jacob@truenorthstrategyops.com
- **Location**: Colorado Springs, CO
- **Certification**: VOSB/SDVOSB

### Colors
- **Navy (primary)**: #1a3a5c - Headers, primary text
- **Teal (accent)**: #3d8eb9 - Secondary headers, highlights
- **Light Teal**: #5ba3c8 - Backgrounds, subtle emphasis

### Typography (Word Documents)
- **H1**: Arial, 36pt, Bold, Navy
- **H2**: Arial, 28pt, Bold, Teal
- **H3**: Arial, 24pt, Bold, Navy
- **Body**: Arial, 11pt, Regular, Black
- **Spacing**: 1.15 line spacing, 10pt after paragraphs

---

## The Two Protocols

### Direction Protocol (Sales Process)
5-stage methodology: IDENTIFY → ASSESS → MAP → CHART → LAUNCH

**Key Phrase**: 
> "Direction Protocol gets you clarity. Command Protocol gets you control."

### Command Protocol (Delivery)
Three service offerings:
- **Command Center Build**: $2,500-5,000, 2-4 weeks
- **Battle Rhythm Install**: $2,000-4,000, 2-4 weeks  
- **Command Partner**: $1,000-2,000/month

---

## Document Templates

### Client-Facing Service Documents

**Structure**:
1. Title (service name)
2. Subtitle (who it's for, italicized teal)
3. What This Engagement Is
4. Who This Is For
5. Problems This Removes
6. What You Get
7. Scope & Pricing
8. Prerequisites (if applicable)
9. What Comes Next (if applicable)

**Use for**: Service descriptions, engagement overviews, offering sheets

### Internal Process Documents

**Structure**:
1. Title (process name)
2. Subtitle (Internal Reference Document)
3. Purpose
4. Overview
5. The Process (numbered steps)
6. Decision Points
7. Tools & Resources Needed
8. Common Issues & Solutions
9. Owner (who maintains)

**Use for**: Team processes, workflows, how-to guides

### Standard Operating Procedures (SOPs)

**Structure**:
1. Title (SOP: Process Name)
2. Effective Date / Version / Status
3. Purpose
4. Scope (what's covered / not covered)
5. Roles & Responsibilities
6. Procedure (detailed steps)
7. Quality Checks
8. Exceptions
9. Related Documents
10. Revision History

**Use for**: Repeatable processes requiring consistency

### Diagnostic/Cheat Sheets

**Structure**:
1. Title (what it's for)
2. Subtitle (duration or context)
3. Before You Start (setup, opening script)
4. Sections with Questions (grouped, numbered)
5. Red Flags / Green Flags
6. Next Steps

**Use for**: Call scripts, assessment guides, quick reference

---

## Usage Examples

### Example 1: Service Document

**Request**:
```
"Create a service document for Command Center Build"
```

**Output**:
- Word document with full TNDS branding
- All sections populated with appropriate content
- Saved as: `TNDS_Service_CommandCenterBuild_2026-01-26.docx`
- Download link provided

### Example 2: Internal SOP

**Request**:
```
"Create an SOP for running a MAP session"
```

**Output**:
- Markdown document with structured SOP format
- Detailed procedure steps
- Quality checks and exceptions
- Saved as: `TNDS_SOP_MapSession_2026-01-26.md`

### Example 3: Diagnostic Tool

**Request**:
```
"Create a cheat sheet for the ASSESS stage"
```

**Output**:
- Word document with scripts and questions
- Red/green flags for qualification
- Timing for each section
- Saved as: `TNDS_Diagnostic_AssessStage_2026-01-26.docx`

---

## Voice & Tone Guidelines

### DO

✅ Use direct, clear language
✅ Write in active voice
✅ Use contractions naturally (don't, won't, can't)
✅ Focus on outcomes ("you'll be able to...")
✅ Keep paragraphs short (2-4 sentences)
✅ Front-load important information
✅ Use specific examples

### DON'T

❌ Use emojis (ever)
❌ Use corporate buzzwords (synergy, leverage)
❌ Apologize or hedge unnecessarily
❌ Write long, meandering sentences
❌ Use passive voice
❌ Over-explain simple concepts

### Language Pattern Examples

**Good**:
> "You'll see every job in real-time, so you know when problems happen—not three days later."

**Bad**:
> "Our real-time visibility solution leverages cutting-edge data integration to enhance operational awareness."

**Good**:
> "Fixed scope, fixed price. No surprise invoices."

**Bad**:
> "We offer transparent pricing models with clearly defined deliverables aligned to your unique requirements."

---

## Key Phrases

Use these consistently across documents:

**The Transformation Statement**:
> "Direction Protocol gets you clarity. Command Protocol gets you control. That's how we turn data into direction."

**Value Proposition**:
> "See what's happening in your operation so you can make better decisions and take a day off."

**Pricing Philosophy**:
> "Fixed scope, fixed price. No open-ended projects. No surprise invoices."

**Prerequisites**:
> "Every engagement begins with the Direction Protocol: we Identify fit, Assess your situation, and Map your operation before we build anything."

---

## Command Modules Reference

All modules end in "-command" or "-ops":

**Core Operations**:
- data-command
- office-command
- analytics-command

**Financial**:
- financial-command
- proposal-command
- contract-command

**Field Service**:
- asset-command
- sms-command

**Specialized**:
- onboard-command, workspace-command, realty-command, tax-command, seo-command, govcon-command, compliance-gov-module

---

## ICP (Ideal Client Profile)

**Who We Work With**:
- 5-20 person operations (field service or office)
- Owner overwhelmed, no middle management
- Information scattered (texts, paper, spreadsheets)
- Can't see what's happening in real-time
- Can't take a day off without chaos

**Who We Don't Work With**:
- Startups without operations foundation
- Anyone looking for "AI magic"
- Micromanagers who won't delegate
- No budget authority
- Won't commit to Direction Protocol
- Wrong size (too small or too large)

---

## Integration with Other Skills

Documentation is the "terminal" skill that produces deliverables for all other skills. See [SKILL-INTEGRATIONS.md](SKILL-INTEGRATIONS.md) for complete details.

### Quick Integration Reference

| Skill | Documents Produced |
|-------|-------------------|
| Direction Protocol | ASSESS notes, MAP summary, Proposals, Agreements |
| Command Protocol | Kickoff docs, Training materials, Handoff docs |
| World Model Mapper | Process docs, Gap reports |
| Bearing Check | Decision records, Decision log |
| ARO Assessment | Assessment reports |

### Direction Protocol Skill
When creating docs about Direction Protocol:
- Reference the 5 stages correctly
- Use proper timing (15-20 min, 30 min, etc.)
- Include correct scripts and questions

### World Model Mapper Skill
When creating process docs:
- Reference workflow mapping approaches
- Link to World Mapper outputs appropriately

### Bearing Check Skill
When documenting decisions:
- Use decision record template
- Reference checkpoint findings
- Log in decision tracker

---

## File Naming Conventions

**Format**: `TNDS_[Type]_[Name]_[Date].ext`

**Type Codes**:
- Service (client-facing service doc)
- Proposal (client proposal)
- Agreement (service agreement)
- SOP (standard operating procedure)
- Process (internal process doc)
- Diagnostic (cheat sheet/tool)
- Spec (technical specification)
- Training (training materials)

**Examples**:
- `TNDS_Service_CommandCenterBuild_2026-01-26.docx`
- `TNDS_SOP_ClientOnboarding_2026-01-26.md`
- `TNDS_Diagnostic_AssessCheatSheet_2026-01-26.docx`

---

## Quality Checklist

Before finalizing any document:

**Content**:
- [ ] Voice matches TNDS tone (direct, no-fluff)
- [ ] Uses outcomes language
- [ ] Specific and concrete
- [ ] Key phrases used correctly
- [ ] No jargon without definition
- [ ] No emojis

**Structure**:
- [ ] Follows appropriate template
- [ ] Logical flow and organization
- [ ] Headers create clear hierarchy
- [ ] Bullets used appropriately

**Formatting (Word)**:
- [ ] Logo in header (centered)
- [ ] Footer formatted correctly
- [ ] Colors correct (Navy/Teal)
- [ ] Font sizes match spec
- [ ] Spacing consistent

**Completeness**:
- [ ] All required sections present
- [ ] Contact info correct
- [ ] Pricing accurate (if applicable)
- [ ] Timeline realistic (if applicable)

---

## Common Mistakes to Avoid

### Voice Mistakes
❌ "Our cutting-edge solution leverages AI-powered automation..."
✅ "You'll see every job in real-time and know when problems happen"

### Structure Mistakes
❌ Bury important information in third paragraph
✅ Lead with what matters most

❌ Write 8-sentence paragraphs
✅ Keep paragraphs to 2-4 sentences

### Formatting Mistakes
❌ Mix fonts or use random colors
✅ Stick to Arial, Navy, Teal, Black, Gray

❌ Underline for emphasis
✅ Use bold for emphasis

---

## Quick Reference Commands

| You Say | Claude Creates |
|---------|---------------|
| "Create service doc for [name]" | Client-facing service document |
| "Create SOP for [process]" | Standard operating procedure |
| "Create internal process doc" | Internal how-to guide |
| "Create cheat sheet for [stage]" | Diagnostic assessment tool |
| "Document [module] module" | Module documentation |
| "Generate proposal for [client]" | Client proposal |
| "Create agreement for [service]" | Service agreement |

---

## Tips for Best Results

### 1. Be Specific
Don't just say "create a document." Specify:
- Document type (service doc, SOP, cheat sheet)
- Topic/service it covers
- Audience (client-facing, internal, technical)

### 2. Provide Context
Give Claude information about:
- What the service/process is
- Who it's for
- What problem it solves
- Key details (pricing, timeline, etc.)

### 3. Request Format
Specify if you want:
- Word document (`.docx`) - best for client-facing
- Markdown (`.md`) - best for internal/technical
- Both formats

### 4. Iterate
Claude can refine documents based on feedback:
- "Make it more concise"
- "Add a section about..."
- "Change the tone to be more..."

---

## Support & Updates

### Updating This Skill
To modify branding, voice, or templates:
1. Edit `SKILL.md`
2. Update version number
3. Test with sample documents
4. Deploy updated skill

### Questions or Issues
- Review examples in `examples.md`
- Check voice guidelines in `SKILL.md`
- Refer to document tools in `document-tools.md`

### Version History

**v1.1** (2026-01-29)
- Added WORKFLOW.md (step-by-step process)
- Added SKILL-INTEGRATIONS.md (cross-skill integration)
- Added QUALITY-REVIEW-CHECKLIST.md (quality standards)
- Added TRAINING-GUIDE.md (onboarding)
- Added CASE-STUDIES.md (worked examples)
- Added EMAIL-TEMPLATES.md (communication templates)
- Added PROPOSAL-TEMPLATE.md (detailed proposal guide)
- Added AGREEMENT-TEMPLATE.md (service agreement guide)
- Added MODULE-DOCUMENTATION-TEMPLATE.md (module docs)
- Added FOLDER-STRUCTURE.md (file organization)
- Added METRICS-DASHBOARD.md (tracking metrics)
- Updated README.md with new document references

**v1.0** (2026-01-26)
- Initial release
- Full branding system
- All document templates
- Voice & tone guidelines
- Python generation tools

---

## Technical Details

### Dependencies
- python-docx (for Word document generation)
- Python 3.8+ (for script execution)

### Output Location
All documents are saved to: `/mnt/user-data/outputs/`

### Logo File
Located at: `/mnt/user-data/uploads/word-doc-tnds-logo.png` or  `./word-doc-tnds-logo.png` in skill directory

---

## Real-World Workflow Example

**Monday**: Need to document new service
1. "Create service document for Battle Rhythm Install"
2. Claude generates Word doc with full branding
3. Review and request refinements
4. Download final version
5. Share with prospects

**Tuesday**: Need internal SOP
1. "Create SOP for handling client change requests"
2. Claude generates Markdown SOP
3. Add to internal wiki
4. Team now has consistent process

**Wednesday**: Need diagnostic tool
1. "Create cheat sheet for MAP session"
2. Claude generates Word doc with scripts
3. Print for reference during calls
4. Sales team uses during discovery

---

## Summary

This skill ensures every TNDS document maintains:
- ✅ Consistent brand identity
- ✅ Professional formatting
- ✅ Clear, direct voice
- ✅ Appropriate structure
- ✅ High-quality content

Whether creating client-facing proposals or internal SOPs, the TNDS Documentation skill delivers professional, on-brand documents every time.

---

**Contact**: Jacob Johnston | 719-204-6365 | jacob@truenorthstrategyops.com

**Company**: True North Data Strategies • Colorado Springs, CO
---

© 2026 True North Data Strategies LLC. Licensed under MIT — see LICENSE.

*Direction Protocol™, Command Protocol™, Battle Rhythm Install™, Command Center Build™, Bearing Check™, World Model Mapper™, and ARO Assessment™ are trademarks of True North Data Strategies LLC.*

---

**END OF README**
