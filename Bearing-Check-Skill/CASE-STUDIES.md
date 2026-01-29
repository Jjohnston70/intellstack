# Bearing Check Case Studies

**Version:** 1.0
**Last Updated:** January 29, 2026
**Purpose:** Real-world examples of Bearing Check decision validation in action

---

## Overview

These case studies demonstrate how the Bearing Check framework applies to different decision types. Each case shows:
- The decision context
- How each checkpoint was evaluated
- What was discovered
- The final recommendation and outcome

---

## Case Study 1: New Vertical Entry

### Decision: Should TNDS Launch a Restaurant-Command Module?

**Context:** After successfully building Command Centers for field service operations, the idea arose to expand into restaurant operations. Several restaurant owners had expressed interest. The question: Is this a good investment of time and resources?

**Stakes:**
- Time at risk: 200+ hours to develop module
- Capital at risk: $5,000-10,000 opportunity cost
- Reversibility: Partially reversible (could sunset if unsuccessful)

---

#### Checkpoint 1: Ground Truth

**Question:** How often do consultants successfully add new verticals?

**Finding:** Research revealed:
- 30-40% of consulting firms that add new verticals achieve profitability in that vertical within 2 years
- Success rate drops to ~20% when the new vertical has different buyer personas
- Restaurant tech specifically has high churn—60% of restaurant tech startups fail within 3 years

**Flag:** 🟡 Yellow — Base rate is concerning but not fatal

---

#### Checkpoint 2: Graveyard Recon

**Question:** Who tried restaurant operations consulting and failed?

**Finding:** Found multiple patterns in failures:
- Consultants who underestimated industry-specific complexity (POS systems, health codes, labor laws)
- Those who assumed "operations are operations" without understanding restaurant-specific workflows
- Tech solutions that didn't account for high staff turnover and training needs
- Margin sensitivity—restaurants operate on 3-5% margins, less room for automation investment

**Flag:** 🔴 Red — Multiple failure patterns apply to TNDS

---

#### Checkpoint 3: Mechanism Check

**Question:** Why does Command Center work for field service?

**Finding:** The mechanism that makes field service work:
- Dispatching, scheduling, and job costing are **universal** across HVAC, plumbing, electrical
- Owner pain is **visibility** (same regardless of trade)
- TNDS has **direct experience** in field service operations

For restaurants, the mechanism would need to be different:
- Inventory, labor scheduling, and table management are restaurant-specific
- Owner pain is **margins** more than visibility
- TNDS has **no direct experience** in restaurant operations

**Flag:** 🔴 Red — Mechanism doesn't transfer

---

#### Checkpoint 4: Fixed Points

**Question:** Are the success factors durable?

**Finding:**
- **Fixed (Durable):** Operational efficiency need, data visibility desire
- **Situational:** Restaurant-specific integrations (Toast, Square, etc.), industry relationships, understanding of restaurant workflows

The durable factors are generic; the situational factors are critical and missing.

**Flag:** 🟡 Yellow — Fixed points present but insufficient

---

#### Checkpoint 5: Odds Assessment

**Question:** What are realistic odds?

**Finding:**
- Without restaurant experience: 10-20% success
- With industry partner: 30-40% success
- Time to profitability: 18-24 months minimum
- Downside: 200+ hours lost, brand dilution if done poorly

**Flag:** 🔴 Red — Odds don't justify investment

---

#### Checkpoint 6: Constraint Fit

**Constraint Analysis:**

| Constraint | Reality | Requirement | Match? |
|------------|---------|-------------|--------|
| Industry expertise | None | High | ❌ |
| Time available | Limited | Significant | ⚠️ |
| Capital | Adequate | Moderate | ✅ |
| Network in industry | None | Important | ❌ |
| Risk tolerance | Moderate | High risk venture | ⚠️ |

**Flag:** 🔴 Red — Major constraint mismatches

---

#### Checkpoint 7: Staged Advance

**Proposed Stages:**
- Stage 1: Partner with one restaurant owner informally (10 hours)
- Stage 2: Build prototype for that single restaurant (40 hours)
- Stage 3: Test with 2-3 more restaurants (100 hours)

**Problem:** Even Stage 1 requires learning a new industry while current field service demand is strong.

**Flag:** 🟡 Yellow — Staged approach exists but competes with core business

---

#### Checkpoint 8: Pre-Mortem

**Failure Narrative:**
> "It's January 2027. The restaurant-command module failed. Here's what happened: We spent 6 months building something that looked like our field service solution but didn't fit restaurant workflows. Our first client churned after 3 months because the labor scheduling didn't integrate with their existing POS. We discovered too late that restaurants need real-time inventory, not just tracking. The margins in restaurant consulting were too thin to support our pricing model. Meanwhile, we lost two field service clients because we were distracted."

**Survivability:** Financially survivable but damaging to focus

**Flag:** 🔴 Red — Failure mode is realistic and costly

---

### Final Bearing

| Checkpoint | Finding | Flag |
|------------|---------|------|
| 1. Ground Truth | 30-40% success rate, lower for new personas | 🟡 |
| 2. Graveyard Recon | Multiple failure patterns apply directly | 🔴 |
| 3. Mechanism Check | Core mechanism doesn't transfer | 🔴 |
| 4. Fixed Points | Durable factors insufficient | 🟡 |
| 5. Odds Assessment | 10-20% success, 18-24 month timeline | 🔴 |
| 6. Constraint Fit | Major mismatches (expertise, network) | 🔴 |
| 7. Staged Advance | Possible but competes with core | 🟡 |
| 8. Pre-Mortem | Realistic failure, costly distraction | 🔴 |

**Recommendation:** NO-GO

**Confidence:** High

**Rationale:** Five red flags across eight checkpoints. The mechanism that makes field service work doesn't transfer to restaurants. Constraint fit is poor—no industry expertise or network. The opportunity cost of distraction from a working business is significant.

**Alternative Path:** If a restaurant opportunity appears, refer to a partner rather than build in-house.

---

## Case Study 2: Partnership Opportunity

### Decision: Should TNDS Partner with an MSP for Joint Service Delivery?

**Context:** A local Managed Service Provider (MSP) approached TNDS about partnering. They handle IT; TNDS would handle operational systems. Potential to share clients and expand reach.

**Stakes:**
- Time at risk: 20-40 hours to establish partnership
- Revenue share: TBD
- Reversibility: Easily reversible if partnership doesn't work

---

#### Checkpoint 1: Ground Truth

**Question:** How often do small consulting partnerships succeed?

**Finding:**
- Research indicates 50-60% of small business partnerships dissolve within 2 years
- Success factors: clear scope, complementary (not competitive) services, aligned values
- MSP-operations partnerships specifically: limited data, but adjacent service model

**Flag:** 🟡 Yellow — Moderate base rate, need to mitigate risks

---

#### Checkpoint 2: Graveyard Recon

**Question:** Why do consulting partnerships fail?

**Finding:**
- Unclear lead ownership (who "owns" the client)
- Misaligned service quality standards
- Scope creep into each other's territory
- Unequal effort/unequal revenue sharing
- One partner outgrows the other

**Flag:** 🟢 Green — Failure modes are addressable with clear agreements

---

#### Checkpoint 3: Mechanism Check

**Question:** Why would this partnership work?

**Finding:**
- MSP has IT clients who need operations help (clear referral path)
- TNDS has operations clients who need IT help (reciprocal referral)
- Services are complementary, not competitive
- Both work with similar client size (5-20 person operations)

**Mechanism:** Referral exchange with aligned client profiles

**Flag:** 🟢 Green — Clear mechanism, complementary services

---

#### Checkpoint 4: Fixed Points

**Question:** Are success factors durable?

**Fixed Points:**
- Both serve similar client sizes (durable)
- Services are complementary (durable)
- Geographic proximity (durable)

**Situational:**
- MSP's current client base (could change)
- Relationship quality with MSP owner (depends on ongoing effort)

**Flag:** 🟢 Green — Core factors are stable

---

#### Checkpoint 5: Odds Assessment

**Question:** What are the odds this works?

**Finding:**
- With clear agreement: 50-60% success
- Without clear agreement: 20-30% success
- Upside: 2-4 additional clients per year via referrals
- Downside: Time spent, potential reputation risk if MSP delivers poorly

**Flag:** 🟢 Green — Favorable odds with mitigation

---

#### Checkpoint 6: Constraint Fit

| Constraint | Reality | Requirement | Match? |
|------------|---------|-------------|--------|
| Time available | Limited | Moderate (20-40 hrs) | ✅ |
| Trust in partner | TBD (need to verify) | High | ⚠️ |
| Service alignment | Complementary | Complementary | ✅ |
| Client profile match | Same target | Same target | ✅ |
| Revenue expectations | Referral fees | Referral fees | ✅ |

**Flag:** 🟡 Yellow — Need to verify trust/quality

---

#### Checkpoint 7: Staged Advance

**Proposed Stages:**
- Stage 1: One test referral in each direction (2 weeks, 5 hours)
- Stage 2: Review outcomes, discuss formal arrangement (2 hours)
- Stage 3: Sign referral agreement, commit to quarterly reviews

**Success Signals:**
- Both referrals handled well
- Client feedback positive
- Communication was smooth

**Flag:** 🟢 Green — Clear staged approach

---

#### Checkpoint 8: Pre-Mortem

**Failure Narrative:**
> "The MSP partnership failed after 6 months. The MSP referred a client who was actually a bad fit—they wanted IT support, not operations. When I pushed back, the MSP owner got defensive. We didn't have clear criteria for what makes a good referral. The relationship became awkward and we quietly stopped referring to each other."

**Survivability:** Easily survivable, low cost failure

**Mitigation:** Create clear referral criteria before starting

**Flag:** 🟢 Green — Low-cost failure, mitigatable

---

### Final Bearing

| Checkpoint | Finding | Flag |
|------------|---------|------|
| 1. Ground Truth | 50-60% with clear agreement | 🟡 |
| 2. Graveyard Recon | Failure modes addressable | 🟢 |
| 3. Mechanism Check | Clear complementary mechanism | 🟢 |
| 4. Fixed Points | Core factors stable | 🟢 |
| 5. Odds Assessment | Favorable with mitigation | 🟢 |
| 6. Constraint Fit | Need to verify trust | 🟡 |
| 7. Staged Advance | Clear test path | 🟢 |
| 8. Pre-Mortem | Low-cost, mitigatable | 🟢 |

**Recommendation:** CONDITIONAL GO

**Conditions:**
1. Complete one test referral in each direction before formalizing
2. Create written referral criteria (what makes a good referral)
3. Verify MSP service quality with their existing clients

**Confidence:** Medium-High

**Next Action:** Schedule coffee with MSP owner to discuss test referral

---

## Case Study 3: Quick Bearing Check Example

### Decision: Should I Attend Local Business Networking Event?

**Context:** Invitation to a local chamber of commerce event. $50 registration, 3 hours including travel.

**Stakes:** Low (time and small fee)
**Check Type:** Quick (Checkpoints 1, 5, 8)

---

#### Checkpoint 1: Ground Truth

**Question:** How often do networking events generate clients?

**Finding:** Industry data suggests 5-10% of networking attendees convert a contact into a client within 12 months. However, consistency matters—regular attendees see higher conversion (15-20%).

**Flag:** 🟢 Green — Reasonable expectations

---

#### Checkpoint 5: Odds Assessment

**Question:** What's the expected value?

**Finding:**
- Cost: $50 + 3 hours (~$150 opportunity cost) = $200 total
- If I meet one prospect who converts (5% chance): $2,500 minimum project value
- Expected value: 5% × $2,500 = $125
- Net expected value is negative (-$75) for single event

**However:** Building relationships compounds over time. After 3-4 events, conversion rate increases.

**Flag:** 🟡 Yellow — Single event negative EV, but compounding potential

---

#### Checkpoint 8: Pre-Mortem

**Question:** What if this fails?

**Finding:**
- Worst case: I spend 3 hours and meet no one useful
- Survivability: Easily survivable (it's 3 hours)
- Repeatability: Yes, this is a repeatable activity

**Flag:** 🟢 Green — Low-cost failure

---

### Quick Bearing

**Recommendation:** CONDITIONAL GO

**Condition:** Commit to attending 3-4 events before judging ROI (compounding effect)

**Confidence:** Medium

**Next Action:** Register, set calendar reminder for 3 more events

---

## Case Study 4: NO-GO That Saved Resources

### Decision: Should I Build a SaaS Product Instead of Services?

**Context:** Recurring thought about building a productized SaaS version of Command Center instead of custom client work. The appeal: passive income, scalability.

**Stakes:**
- Time at risk: 6-12 months of development
- Capital at risk: $20,000-50,000
- Opportunity cost: All client work during development

---

#### Checkpoint 1: Ground Truth

**Question:** What's the success rate for solo-founder SaaS?

**Finding:**
- 90% of SaaS startups fail
- Solo founders have ~5% chance of reaching $10K MRR within 3 years
- Average time to profitability (for those who succeed): 18-36 months

**Flag:** 🔴 Red — Base rate is very poor

---

#### Checkpoint 2: Graveyard Recon

**Question:** Why do solo-founder SaaS products fail?

**Finding:**
- Building before validating demand (most common)
- Running out of runway before product-market fit
- Underestimating sales/marketing effort
- Feature creep and scope expansion
- Competition from funded startups

**Pattern that applies:** TNDS already has proven demand for services. Building SaaS would mean walking away from validated demand for unvalidated demand.

**Flag:** 🔴 Red — Multiple failure patterns apply

---

#### Checkpoint 5: Odds Assessment

**Question:** What are realistic odds?

**Finding:**
- Success probability: 5-10%
- Time to break-even: 2-3 years (if successful)
- Current services revenue at risk: $100K+ during development
- Downside: Broke, burned out, lost existing client relationships

**Flag:** 🔴 Red — Terrible risk/reward

---

### Quick Bearing (stopped early due to red flags)

**Recommendation:** NO-GO

**Confidence:** High

**Rationale:** The base rate for solo-founder SaaS is 5-10% success. Current services business has near-100% success rate per engagement. Trading a working business for a long-shot is irrational.

**Alternative Path:** Continue services; consider productized service offerings (fixed scope packages) if scalability is the goal.

**Lesson:** The Bearing Check stopped at checkpoint 5 because three consecutive red flags made further analysis unnecessary. This saved time that would have been spent rationalizing a bad idea.

---

## Patterns Across Case Studies

### When Bearing Check Says NO-GO

Common patterns in NO-GO decisions:
- Base rate is poor AND constraints don't fit
- Mechanism doesn't transfer from source to your situation
- Pre-mortem reveals non-survivable failure
- Multiple red flags (3+) across checkpoints

### When Bearing Check Says GO

Common patterns in GO decisions:
- Base rate is reasonable (30%+)
- Mechanism is understood and applicable
- Constraints fit or can be addressed
- Staged approach exists
- Failure is survivable

### When to Stop Early

Stop the Bearing Check early if:
- Three consecutive red flags appear
- Base rate + Graveyard Recon both red = don't proceed
- Constraint mismatch is fundamental (can't be fixed)

### The Value of Quick Checks

Quick Bearing Checks (checkpoints 1, 5, 8) are sufficient when:
- Stakes are moderate
- Pattern is familiar
- Time pressure exists
- You need a sanity check, not full validation

---

## Applying These Patterns

### Before Your Next Bearing Check

1. **Identify the pattern:** Which case study is most similar to your decision?
2. **Focus on mechanisms:** Why did that example work or fail?
3. **Watch for red flag clustering:** Multiple reds = stop early
4. **Document for future:** Your decisions become case studies

---

**Document Status:** Active
**Next Review:** After 5 more documented decisions
**Feedback:** Add your own case studies to this document

