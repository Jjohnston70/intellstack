# The Bearing Check - User Manual

## What This Is

The Bearing Check is a decision validation framework for Pipeline Punks and TNDS. It helps you (and your audience) pressure-test decisions before committing resources. Think of it as a pre-flight checklist for major life and business decisions.

The framework synthesizes concepts from statistical decision theory, behavioral economics, and risk management into eight sequential checkpoints. The navigation metaphor (bearing check, checkpoints, staged advance) aligns with TNDS brand language.

---

## Folder Structure

```
Bearing_Check/
├── USER_MANUAL.md          <-- You are here
├── skill/
│   ├── SKILL.md            <-- Main skill file (upload to Claude Projects)
│   └── references/
│       ├── checkpoints.md  <-- Detailed examples for each checkpoint
│       ├── cognitive-biases.md  <-- The 7 traps this framework solves
│       └── framework.md    <-- Red flags and navigation approaches
└── archive/
    └── Eight_Gates_original/  <-- Old files before rebranding
```

---

## How to Use the Skill

### Option 1: Claude Project (Recommended)

1. Create a new Claude Project called "Bearing Check" or "Decision Engine"
2. Upload the entire `skill/` folder contents:
   - `SKILL.md` (required)
   - `references/checkpoints.md`
   - `references/cognitive-biases.md`
   - `references/framework.md`
3. Claude will now use this framework when you ask decision-related questions

**Trigger phrases that activate the skill:**
- "Should I..."
- "Is this a good idea..."
- "Help me decide..."
- "Evaluate this strategy..."
- "What are the risks of..."
- "Run a bearing check on..."

### Option 2: Manual Invocation

If the skill isn't loaded, you can paste the SKILL.md content directly into a conversation and ask Claude to run a decision through the eight checkpoints.

### Option 3: Self-Guided

Use the checkpoints.md file as a personal checklist. Work through each checkpoint manually for important decisions.

---

## The Eight Checkpoints (Quick Reference)

| # | Checkpoint | Core Question |
|---|------------|---------------|
| 1 | Ground Truth | What's the actual success rate for people like me? |
| 2 | Graveyard Recon | Who tried this and failed? What happened? |
| 3 | Mechanism Check | What actually caused success? Would it work without hidden factors? |
| 4 | Fixed Points | Which success factors are stable vs. trendy? |
| 5 | Odds Assessment | What are the real odds? What happens if I'm wrong? |
| 6 | Constraint Fit | Do my resources and temperament match this strategy? |
| 7 | Staged Advance | What's the smallest test I can run first? |
| 8 | Pre-Mortem | If I fail, what caused it? Can I survive it? |

---

## When to Use Full vs. Quick Pass

### Full Framework (All 8 Checkpoints)
Use for major decisions with significant downside:
- Career pivots
- Large investments (>10% of savings)
- Business bets
- Partnership commitments
- Hiring key roles
- Major client contracts

### Quick Pass (Checkpoints 1, 5, 7)
Use for smaller decisions where three checks provide sufficient rigor:
- Checkpoint 1: Ground Truth (what's the base rate?)
- Checkpoint 5: Odds Assessment (what are real odds and downside?)
- Checkpoint 7: Staged Advance (can I test before committing?)

### Single Checkpoint
Use when someone asks about a specific aspect:
- "What's the success rate?" → Checkpoint 1 only
- "What could go wrong?" → Checkpoint 8 only

---

## Pipeline Punks Integration

### Content Strategy

1. **Publish the framework** as a Pipeline Punks article or video
2. **Offer the skill** as a member benefit
3. **Collect applications** from members who use it
4. **Create case studies** from anonymized applications

### Teaching Approach

When explaining to Pipeline Punks audience:
- Lead with the problem: "Most people copy winners without understanding why they won"
- Use the navigation metaphor: "Before you commit to a heading, verify your position"
- Emphasize the staged approach: "You don't have to be right immediately. You have to not blow up while learning."

### Example Content Hooks

- "The 8 questions that kill bad business ideas before they kill your savings"
- "Why 'just do it' is terrible advice (and what to do instead)"
- "How to steal strategies without getting burned"
- "The pre-mortem: Why imagining failure makes you more likely to succeed"

---

## TNDS Client Application

The Bearing Check maps to the Direction Protocol:

| Direction Protocol | Bearing Check Equivalent |
|-------------------|-------------------------|
| Identify | Checkpoint 1 (Ground Truth) - Is there actually a problem worth solving? |
| Assess | Checkpoints 2-4 (Recon, Mechanism, Fixed Points) - What's really going on? |
| Map | Checkpoint 6 (Constraint Fit) - What does their specific situation require? |
| Chart | Checkpoints 5, 7 (Odds, Staged Advance) - What's the realistic plan? |
| Launch | Checkpoint 8 (Pre-Mortem) - What could derail this? |

You can use the framework internally during discovery calls to validate whether a prospect's problem is real and solvable.

---

## Reference Files Explained

### checkpoints.md
Detailed breakdown of each checkpoint with:
- What it means
- Key questions to ask
- Example applications
- Common mistakes

**Use when:** You need to teach someone the framework or want detailed examples.

### cognitive-biases.md
The seven cognitive traps the framework counters:
1. Survivorship Bias
2. Winner's Curse
3. Gambling Bias
4. Wrong Variable Selection
5. Ignoring Uncertainty
6. External Validity Problems
7. Non-Stationarity

**Use when:** You need to explain WHY a checkpoint matters or someone is resisting the process.

### framework.md
- Origin and philosophy
- The two navigation approaches (Lost Navigator vs. Bearing Check)
- Red flags for each checkpoint

**Use when:** You need quick red-flag detection or want to explain the overall philosophy.

---

## Customization Options

### For Different Audiences

**Investors/Finance:** Emphasize checkpoints 1, 5, 7, 8 (base rates, odds, staged bets, survivability)

**Career Changers:** Emphasize checkpoints 1, 3, 6 (base rates, mechanism vs. behavior, constraint fit)

**Founders/Builders:** Emphasize checkpoints 2, 4, 7 (failure analysis, stable factors, staged testing)

### Adding Domain-Specific Examples

Edit `checkpoints.md` to add examples relevant to your audience:
- GovCon examples for TNDS prospects
- Tech career examples for Pipeline Punks
- Small business examples for general use

---

## Maintenance

### Updating the Skill

When you want to improve the framework:
1. Edit files in the `skill/` folder
2. Re-upload to Claude Projects
3. Test with sample decisions
4. Keep old versions in `archive/` if needed

### Version History

- v1.0: Original "Eight Gates" framework
- v2.0: Rebranded to "Bearing Check" with checkpoint naming

---

## Attribution

This framework adapts concepts from statistical decision theory and behavioral economics. The original structure was inspired by a Data Science Collective article, then rebranded and adapted for the TNDS/Pipeline Punks context.

When publishing, include a general attribution:
> "The Bearing Check framework synthesizes concepts from statistical decision theory, behavioral economics, and risk management."

You do not need to cite specific sources for the underlying concepts (base rates, survivorship bias, pre-mortems) as these are established public domain ideas.

---

## Quick Start

1. Upload the `skill/` folder to a Claude Project
2. Ask: "Run a bearing check on [your decision]"
3. Work through each checkpoint Claude presents
4. Get a Final Bearing recommendation

That's it. The framework does the heavy lifting.

---

## Legal

**Trademarks:** Direction Protocol™, Command Protocol™, Bearing Check™, World Model Mapper™, ARO Assessment™, Battle Rhythm Install™, and Command Center Build™ are trademarks of True North Data Strategies LLC.

---

© 2026 True North Data Strategies LLC. Licensed under MIT — see LICENSE.
