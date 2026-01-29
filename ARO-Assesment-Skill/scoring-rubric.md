# ARO Scoring Rubric

Detailed criteria for scoring each operational area. Use specific examples from discovery to justify scores.

---

## File Organization (1-5)

### Score 1: Chaotic
- Files named "doc1.docx", "final_final_v2.xlsx", "asdfgh.pdf"
- No folder structure or random folders
- Desktop covered in files
- Multiple versions of same document with no clear current version
- Team members save to different locations
- Finding anything requires asking someone or extensive searching

**AI Impact:** Agent cannot locate relevant files. Every request requires manual file hunting.

### Score 2: Struggling
- Some folders exist but structure is inconsistent
- Naming conventions attempted but not followed
- Can usually find things but takes significant time
- Duplicates exist across locations
- Some files in email attachments only

**AI Impact:** Agent finds wrong versions, misses relevant files, produces inconsistent results.

### Score 3: Functional
- Clear folder hierarchy for most content
- Naming conventions exist, followed ~70% of time
- Can find most things with moderate effort
- Primary location established, some exceptions
- Occasional duplicates but manageable

**AI Impact:** Agent works for common scenarios, fails on edge cases or historical data.

### Score 4: Good
- Consistent folder structure across organization
- Naming conventions documented and followed
- Files findable within minutes
- Single source of truth for most document types
- Some metadata/tagging in use

**AI Impact:** Agent performs well for most tasks. Occasional context gaps.

### Score 5: Agent-Ready
- Hierarchical structure with clear logic
- Consistent naming convention universally followed
- Files self-documenting (name indicates content, date, version)
- Metadata/tags enable sophisticated filtering
- Version control or clear versioning system
- Searchable and browsable with equal effectiveness

**AI Impact:** Agent can locate and reference any relevant file without human intervention.

---

## Process Documentation (1-5)

### Score 1: Tribal Knowledge
- "Ask Sarah" is the documentation
- Nothing written down
- New hires learn by shadowing for weeks
- Processes exist only in people's heads
- Inconsistent execution even for simple tasks

**AI Impact:** Agent has no reference for how work should be done. Cannot assist with process execution.

### Score 2: Minimal
- A few documents exist somewhere
- Written years ago, never updated
- Key processes undocumented
- Documentation scattered across tools
- People don't know docs exist or where they are

**AI Impact:** Agent may find outdated docs, produce incorrect guidance.

### Score 3: Partial
- Core processes documented
- Documentation exists but not maintained (6+ months stale)
- Gaps in coverage (maybe 50% of important processes)
- Some docs high quality, others minimal
- Team knows where to look but docs need interpretation

**AI Impact:** Agent helpful for documented processes, useless for undocumented ones.

### Score 4: Solid
- Most important processes documented (80%+)
- Documentation reviewed/updated quarterly
- Clear ownership of each document
- Consistent format across docs
- New hires can follow docs with minimal questions

**AI Impact:** Agent can guide most standard processes. Some edge cases require human input.

### Score 5: Agent-Ready
- All recurring processes documented
- Step-by-step with decision points explicit
- Version controlled with change history
- Actively maintained (monthly review or trigger-based updates)
- Includes "what to do when things go wrong"
- Machine-readable structure (not just narrative prose)

**AI Impact:** Agent can execute or guide any standard process. Knows when to escalate.

---

## Data Structure (1-5)

### Score 1: Chaos
- Same customer in 5 different spreadsheets with conflicting info
- No central system for anything
- Critical data in email threads
- "Which spreadsheet is current?" is a daily question
- Data entry happens wherever convenient

**AI Impact:** Agent cannot trust any data source. Produces contradictory outputs.

### Score 2: Fragmented
- Primary systems exist but heavily worked around
- Significant data in side spreadsheets
- Sync between systems manual or broken
- Data quality issues acknowledged but not addressed
- "The real info is in [non-system location]"

**AI Impact:** Agent must be told which source to trust for each query.

### Score 3: Centralized but Messy
- Central systems used for most data
- Data quality issues (duplicates, incomplete records, stale data)
- Some integration between systems
- Workarounds exist but are known/documented
- Can usually get accurate info with some effort

**AI Impact:** Agent works but may surface bad data. Requires validation.

### Score 4: Clean
- Single source of truth for each data type
- Data quality actively managed
- Systems integrated where needed
- Minimal workarounds required
- Data entry standards followed

**AI Impact:** Agent can query data confidently. Occasional edge cases.

### Score 5: Agent-Ready
- Single source of truth, universally respected
- Data validation at entry
- Automated sync between systems
- Clear data dictionary/schema
- Historical data accessible and accurate
- API access available for automation

**AI Impact:** Agent can query, analyze, and act on data without human verification.

---

## Decision Logic (1-5)

### Score 1: Person-Dependent
- Every non-trivial decision requires finding the right person
- No documented criteria for any decision
- Answers to "how do we decide X?" vary by who you ask
- Bottlenecks around key decision-makers
- Inconsistent decisions for similar situations

**AI Impact:** Agent cannot make or recommend any decision. Every question escalates.

### Score 2: Informal Guidelines
- Some rules exist but aren't written down
- "We usually do X, but sometimes Y" with no clear when
- Experienced people know the patterns
- New hires struggle to make decisions
- Consistency depends on who's handling it

**AI Impact:** Agent may guess wrong. Outputs not reliable for decision support.

### Score 3: Documented Guidelines
- Key decision criteria documented
- General rules exist with room for judgment
- Most situations covered by guidelines
- Some exceptions require escalation
- Team generally consistent in decisions

**AI Impact:** Agent can suggest decisions for standard scenarios. Escalates edge cases.

### Score 4: Explicit Rules
- Decision trees documented for most scenarios
- Clear escalation paths for exceptions
- Criteria quantified where possible
- Rules reviewed and updated as business changes
- Team follows rules consistently

**AI Impact:** Agent can make most decisions confidently. Clearly identifies exceptions.

### Score 5: Agent-Ready
- If/then logic documented for all recurring decisions
- Thresholds and criteria explicit and quantified
- Exception handling documented
- Rules accessible in machine-readable format
- Feedback loop to improve rules over time

**AI Impact:** Agent can execute decision logic autonomously. Humans review exceptions only.

---

## Communication Records (1-5)

### Score 1: Lost
- Important conversations lost in email/text threads
- No notes from calls or meetings
- "What did we promise them?" requires memory or guessing
- Context from past interactions inaccessible
- Handoffs between team members lose critical info

**AI Impact:** Agent has no context on relationship history. Every interaction starts cold.

### Score 2: Sporadic
- Some notes taken but not systematically
- Email searchable but nothing else is
- Meeting notes happen sometimes
- CRM has some history but incomplete
- Key context in individual inboxes/texts

**AI Impact:** Agent may find partial context. Gaps cause confusion or errors.

### Score 3: Partial Capture
- CRM or system captures significant history
- Most emails logged or accessible
- Meeting notes taken for important meetings
- Can usually reconstruct timeline with effort
- Some channels (text, calls) still dark

**AI Impact:** Agent can reference recent history. Older context or non-email channels missing.

### Score 4: Good History
- Most interactions logged in searchable system
- Meeting notes standard practice
- Communication channels consolidated or synced
- Timeline reconstructable for most clients/projects
- Handoffs include context transfer

**AI Impact:** Agent can personalize based on history. Some gaps in older records.

### Score 5: Agent-Ready
- Complete interaction history in queryable format
- All channels captured (email, calls, meetings, chat)
- Structured notes with key decisions/commitments tagged
- Searchable by topic, date, person, outcome
- Proactive context surfacing (not just storage)

**AI Impact:** Agent has full context for any interaction. Can reference past discussions naturally.

---

## Access & Permissions (1-5)

### Score 1: Unknown
- Shared passwords common
- No clear record of who has access to what
- Former employees may still have access
- Admin access distributed without tracking
- "Everyone just uses my login"

**AI Impact:** Cannot implement AI tools safely. Security risk blocks automation.

### Score 2: Basic
- Individual accounts exist
- Basic permission levels (admin/user)
- Admin access unclear or over-distributed
- No API strategy
- Manual access changes (often forgotten)

**AI Impact:** AI tools deployable but integration limited. Manual intervention for data access.

### Score 3: Controlled
- Clear permission structure
- Admin access limited and documented
- Most systems properly provisioned
- Some API access available
- Access reviews happen (annually at least)

**AI Impact:** AI tools can connect to some systems. Others require workarounds.

### Score 4: Managed
- Permission matrix documented
- Role-based access implemented
- API keys available for key systems
- Access provisioning/deprovisioning process exists
- Regular access reviews

**AI Impact:** AI tools integrate with most systems. Clear path for new integrations.

### Score 5: Agent-Ready
- Complete access matrix maintained
- API keys managed securely with rotation
- Service accounts for automation
- Principle of least privilege implemented
- Audit trail of access and changes
- Self-service access requests with approval workflow

**AI Impact:** AI agents can be granted precise access needed. Security maintained at scale.

---

## Calculating Overall Score

**Simple average:** Add all six scores, divide by 6.

**Weighted average (recommended):** Weight by importance to their specific goals:

| If primary goal is... | Weight higher: |
|-----------------------|----------------|
| AI chat assistance | Data Structure, Decision Logic |
| Document automation | File Organization, Process Documentation |
| Customer communication | Communication Records, Data Structure |
| Internal operations | Process Documentation, Decision Logic |
| Full automation | Access & Permissions, all others equal |

**Interpretation:**

| Average Score | Agent Readiness Level | Typical Recommendation |
|---------------|----------------------|------------------------|
| 1.0 - 2.0 | Critical gaps | Major restructuring needed before AI tools will help |
| 2.1 - 3.0 | Foundational work needed | Address top 2-3 gaps, then reassess |
| 3.1 - 3.5 | Approaching ready | Targeted improvements, quick wins available |
| 3.6 - 4.0 | Good foundation | Refinements will unlock significant value |
| 4.1 - 5.0 | Agent-ready | Optimization and expansion opportunities |
