---
layout: default
title: "Risk and Problem Solving"
---

# Risk & Problem Solving

> *"Everyone has a plan until they get punched in the mouth."*  
> — Mike Tyson


Complete these topics before entering production. Return to them when risks materialize or when uncertainty increases.

---

# 6A.1 Risk Register — Development

## Why It Matters

Unidentified risks become crises. Identified risks become manageable problems. A risk register transforms vague anxieties into explicit, trackable items with owners and mitigation plans. Without one, teams are perpetually surprised by predictable problems—missed dependencies, technical debt, resource gaps—that derail schedules and morale.

## Framework: Risk Register Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                    DEVELOPMENT RISK REGISTER                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  RISK CATEGORIES                                                    │
│  ├── TECHNICAL — Architecture, performance, integration, tools     │
│  ├── RESOURCE — People, skills, capacity, budget                   │
│  ├── SCHEDULE — Dependencies, milestones, external deadlines       │
│  ├── SCOPE — Creep, ambiguity, changing requirements               │
│  ├── EXTERNAL — Platform, partners, market, regulatory             │
│  └── QUALITY — Bugs, polish, certification, performance            │
│                                                                     │
│  FOR EACH RISK:                                                     │
│  ├── ID + Name (unique identifier)                                 │
│  ├── Category (from above)                                         │
│  ├── Description (what could happen)                               │
│  ├── Likelihood (1-5 scale)                                        │
│  ├── Impact (1-5 scale)                                            │
│  ├── Risk Score (Likelihood × Impact)                              │
│  ├── Mitigation (what we're doing to prevent/reduce)               │
│  ├── Contingency (what we'll do if it happens)                     │
│  ├── Owner (who's watching this risk)                              │
│  ├── Status (Open / Mitigating / Monitoring / Closed / Occurred)   │
│  └── Last Updated (recency of assessment)                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Development Risk Register Template

| ID | Risk Name | Category | Description | L | I | Score | Mitigation | Contingency | Owner | Status |
|----|-----------|----------|-------------|---|---|-------|------------|-------------|-------|--------|
| R001 | | | | | | | | | | |
| R002 | | | | | | | | | | |
| R003 | | | | | | | | | | |
| R004 | | | | | | | | | | |
| R005 | | | | | | | | | | |
| R006 | | | | | | | | | | |
| R007 | | | | | | | | | | |
| R008 | | | | | | | | | | |

**Likelihood Scale:**
- 1 = Rare (<10% chance)
- 2 = Unlikely (10-25%)
- 3 = Possible (25-50%)
- 4 = Likely (50-75%)
- 5 = Almost certain (>75%)

**Impact Scale:**
- 1 = Minimal (absorbed easily)
- 2 = Minor (noticeable but manageable)
- 3 = Moderate (requires adjustment)
- 4 = Major (threatens milestone)
- 5 = Critical (threatens project)

## Framework: Common Development Risks Starter List

Use this as a prompt—not all will apply, and you'll have project-specific risks:

### Technical Risks

| Risk | Typical Triggers | Mitigation Approaches |
|------|------------------|----------------------|
| **Architecture won't scale** | First large-scale test, load testing | Early proof of concept, architecture review |
| **Integration complexity** | Multiple systems touching same data | Clear interfaces, integration sprints |
| **Performance targets unmet** | Art/feature ambitions vs. device specs | Budget early, profile often, escalate fast |
| **Tech debt accumulation** | Speed over quality pressure | Refactor sprints, debt tracking |
| **Tooling inadequate** | Content team blocked, slow iteration | Tool investment early, automation |

### Resource Risks

| Risk | Typical Triggers | Mitigation Approaches |
|------|------------------|----------------------|
| **Key person departure** | Single expert on critical system | Cross-training, documentation, redundancy |
| **Skill gaps discovered** | New technology, unfamiliar platform | Training, hiring, outsourcing |
| **Team capacity insufficient** | Scope vs. timeline math | Realistic planning, early hiring |
| **Budget overrun** | Scope creep, underestimation | Contingency buffer, regular tracking |
| **Outsource quality issues** | First deliveries don't meet bar | Clear briefs, early samples, oversight |

### Schedule Risks

| Risk | Typical Triggers | Mitigation Approaches |
|------|------------------|----------------------|
| **Dependency delays** | Backend, platform, partner not ready | Buffer time, alternative plans |
| **Estimation optimism** | Unknown complexity, new tech | Reference-based estimates, add contingency |
| **Milestone slippage** | Early misses compound | Early warning systems, scope flexibility |
| **External deadline fixed** | Holiday launch, platform event | Work backward, protect buffer |
| **Approval cycles slow** | Platform certification, stakeholders | Start early, build relationships |

### Quality Risks

| Risk | Typical Triggers | Mitigation Approaches |
|------|------------------|----------------------|
| **Bug backlog grows faster than fixed** | Feature velocity outpaces QA | Increase QA, reduce feature rate |
| **Crash rates unacceptable** | Device diversity, edge cases | Broader device testing, crash reporting |
| **First-time user experience broken** | Features built, onboarding neglected | FTUE priority, fresh-eyes testing |
| **Localization delays** | Late strings, translation quality | Early string freeze, quality review |

## Framework: Risk Review Cadence

| Review Type | Frequency | Participants | Purpose |
|-------------|-----------|--------------|---------|
| **Quick scan** | Weekly | Producer + leads | New risks, status changes |
| **Full review** | Bi-weekly | Core team | Re-score all, add/close risks |
| **Milestone review** | Per milestone | Team + stakeholders | Reset for next phase |
| **Deep dive** | Monthly | Risk owners | Top 5 risks detailed review |

## Framework: Risk Escalation Criteria

| Risk Score | Classification | Action Required |
|------------|----------------|-----------------|
| 1-4 | Low | Monitor, review monthly |
| 5-9 | Medium | Active mitigation, review bi-weekly |
| 10-15 | High | Escalate to leadership, review weekly |
| 16-20 | Critical | Immediate action, daily monitoring |
| 21-25 | Severe | Stop other work, all-hands resolution |

## Checklist

- [ ] Risk register created with all categories represented
- [ ] Initial risks identified (aim for 15-25 to start)
- [ ] Likelihood and impact scored for each
- [ ] Mitigation and contingency plans documented
- [ ] Owner assigned for each risk
- [ ] Review cadence established
- [ ] Escalation thresholds defined
- [ ] Register accessible to all team members

## Tasks

1. **Brainstorm risks by category** — Timebox 30 min per category with relevant leads
2. **Score initial risks** — Use calibration examples to norm scores
3. **Identify top 5** — These get the most attention
4. **Assign owners** — Not the producer for everything—distribute
5. **Schedule first review** — Put it on the calendar now
6. **Share with team** — Visibility reduces anxiety and surfaces more risks

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.2 Likelihood × Impact Matrix

## Why It Matters

Not all risks are equal, but they can feel equally urgent in the moment. A Likelihood × Impact matrix provides a visual, objective way to prioritize risks. It prevents the team from spending energy on unlikely minor issues while ignoring probable catastrophes. It also creates a shared language for discussing risk severity.

## Framework: The Risk Matrix

```
                              IMPACT
                 1          2          3          4          5
              Minimal    Minor    Moderate    Major    Critical
           ┌──────────┬──────────┬──────────┬──────────┬──────────┐
         5 │    5     │    10    │    15    │    20    │    25    │
   Almost  │  MEDIUM  │   HIGH   │   HIGH   │ CRITICAL │  SEVERE  │
   Certain │          │          │          │          │          │
           ├──────────┼──────────┼──────────┼──────────┼──────────┤
         4 │    4     │    8     │    12    │    16    │    20    │
   Likely  │   LOW    │  MEDIUM  │   HIGH   │ CRITICAL │ CRITICAL │
           │          │          │          │          │          │
L          ├──────────┼──────────┼──────────┼──────────┼──────────┤
I        3 │    3     │    6     │    9     │    12    │    15    │
K Possible │   LOW    │  MEDIUM  │  MEDIUM  │   HIGH   │   HIGH   │
E          │          │          │          │          │          │
L          ├──────────┼──────────┼──────────┼──────────┼──────────┤
I        2 │    2     │    4     │    6     │    8     │    10    │
H Unlikely │   LOW    │   LOW    │  MEDIUM  │  MEDIUM  │   HIGH   │
O          │          │          │          │          │          │
O          ├──────────┼──────────┼──────────┼──────────┼──────────┤
D        1 │    1     │    2     │    3     │    4     │    5     │
     Rare  │   LOW    │   LOW    │   LOW    │   LOW    │  MEDIUM  │
           │          │          │          │          │          │
           └──────────┴──────────┴──────────┴──────────┴──────────┘
```

## Framework: Calibrating Your Scales

### Likelihood Calibration Examples

| Score | Description | Example Frequency | Project Example |
|-------|-------------|-------------------|-----------------|
| 1 - Rare | Extremely unlikely | <1 in 10 projects | Meteor strikes server facility |
| 2 - Unlikely | Could happen but unusual | 1-2 in 10 projects | Key vendor goes bankrupt |
| 3 - Possible | Has happened before | 3-5 in 10 projects | Platform changes certification requirements |
| 4 - Likely | More likely than not | 5-7 in 10 projects | Initial estimates were optimistic |
| 5 - Almost Certain | Expect it to happen | 8+ in 10 projects | Bug backlog will grow during crunch |

### Impact Calibration Examples

| Score | Description | Schedule Impact | Budget Impact | Quality Impact |
|-------|-------------|-----------------|---------------|----------------|
| 1 - Minimal | Absorbed easily | <1 week delay | <5% overrun | Minor polish issues |
| 2 - Minor | Noticeable | 1-2 week delay | 5-10% overrun | Some bugs ship |
| 3 - Moderate | Requires adjustment | 2-4 week delay | 10-20% overrun | Feature cut or scaled |
| 4 - Major | Threatens milestone | 1-2 month delay | 20-40% overrun | Major feature dropped |
| 5 - Critical | Threatens project | 3+ month delay | 40%+ overrun | Launch compromised |

## Framework: Project-Specific Calibration

Complete this for your project:

**Impact Level 3 (Moderate) for our project means:**

| Dimension | Definition for Our Project |
|-----------|---------------------------|
| Schedule | |
| Budget | |
| Quality | |
| Team | |
| Market | |

**Likelihood Level 3 (Possible) for our project means:**

| Description | Example |
|-------------|---------|
| | |

## Framework: Response Strategy by Zone

| Zone | Score Range | Strategy | Review Frequency | Example Actions |
|------|-------------|----------|------------------|-----------------|
| **SEVERE** | 21-25 | Avoid or Transfer | Daily | Cancel feature, get insurance, restructure |
| **CRITICAL** | 16-20 | Immediate Mitigation | 2-3x/week | Assign senior resources, add contingency |
| **HIGH** | 10-15 | Active Mitigation | Weekly | Implement prevention, prepare contingency |
| **MEDIUM** | 5-9 | Monitor & Mitigate | Bi-weekly | Track triggers, low-cost prevention |
| **LOW** | 1-4 | Accept & Monitor | Monthly | Document, check occasionally |

## Framework: Risk Response Types

| Response Type | When to Use | Example |
|---------------|-------------|---------|
| **Avoid** | High impact, can redesign around | Remove dependency on unreliable partner |
| **Transfer** | Can shift risk to another party | Insurance, outsource with guarantees |
| **Mitigate** | Can reduce likelihood or impact | Add redundancy, increase testing |
| **Accept** | Low score, mitigation cost > benefit | Document and monitor |
| **Exploit** | Positive risk (opportunity) | Accelerate timeline if competitor delays |

## Framework: Your Risk Map

Plot your current risks on this matrix:

```
                              IMPACT
                 1          2          3          4          5
           ┌──────────┬──────────┬──────────┬──────────┬──────────┐
         5 │          │          │          │          │          │
           │          │          │          │          │          │
           ├──────────┼──────────┼──────────┼──────────┼──────────┤
         4 │          │          │          │          │          │
           │          │          │          │          │          │
L          ├──────────┼──────────┼──────────┼──────────┼──────────┤
I        3 │          │          │          │          │          │
K          │          │          │          │          │          │
E          ├──────────┼──────────┼──────────┼──────────┼──────────┤
L        2 │          │          │          │          │          │
I          │          │          │          │          │          │
H          ├──────────┼──────────┼──────────┼──────────┼──────────┤
O        1 │          │          │          │          │          │
O          │          │          │          │          │          │
D          └──────────┴──────────┴──────────┴──────────┴──────────┘

Risk IDs in each cell: _____________________________________________
```

## Framework: Risk Migration Tracking

Track how risks move over time:

| Risk ID | Initial Score | Current Score | Direction | Reason for Change |
|---------|---------------|---------------|-----------|-------------------|
| | | | ↑ ↓ → | |
| | | | ↑ ↓ → | |
| | | | ↑ ↓ → | |

## Checklist

- [ ] Likelihood scale calibrated with project-specific examples
- [ ] Impact scale calibrated with project-specific thresholds
- [ ] All risks plotted on matrix
- [ ] Response strategy assigned by zone
- [ ] Response type chosen for high-scoring risks
- [ ] Risk map visible to team
- [ ] Migration tracking established

## Tasks

1. **Calibrate your scales** with the team—agreement on what "3" means
2. **Plot all risks** from your risk register
3. **Identify clusters** — where are risks concentrating?
4. **Assign response strategies** for top-right quadrant
5. **Create visual** — post in team space or shared doc
6. **Review monthly** — track migrations

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.3 Key Person Dependency Mapping

## Why It Matters

Every team has heroes—people whose departure would create chaos. The hero who knows the entire backend architecture. The artist who understands the style guide intuitively. The producer who holds all the relationships. These single points of failure are existential risks hiding in plain sight. Mapping them enables deliberate redundancy before it's urgently needed.

## Framework: Dependency Categories

```
┌─────────────────────────────────────────────────────────────────────┐
│                    KEY PERSON DEPENDENCY TYPES                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  🧠 KNOWLEDGE — Unique understanding not documented                 │
│  ├── System architecture mental model                               │
│  ├── Historical decision context ("why we did X")                   │
│  ├── Undocumented edge cases and workarounds                        │
│  └── Tribal knowledge about codebase quirks                         │
│                                                                     │
│  🛠️ SKILL — Rare capability not easily replaced                     │
│  ├── Specialized technical expertise                                │
│  ├── Tool mastery (proprietary or complex)                          │
│  ├── Artistic style/sensibility that defines the game               │
│  └── Domain expertise (e.g., real-world military advisor)           │
│                                                                     │
│  🔑 ACCESS — Credentials, relationships, permissions                │
│  ├── Platform relationships and contacts                            │
│  ├── Vendor relationships                                           │
│  ├── Admin access to critical systems                               │
│  └── Stakeholder trust and influence                                │
│                                                                     │
│  ⏱️ CAPACITY — Work only they can do fast enough                    │
│  ├── Bottleneck skills (only animator, only sound designer)         │
│  ├── Review/approval authority                                      │
│  └── Context-switching cost if shared                               │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Key Person Dependency Audit

### Step 1: Identify Critical Areas

| Area | What Would Break | Who Knows This Best | Backup Available? |
|------|------------------|---------------------|-------------------|
| Backend architecture | | | Y / N / Partial |
| Build/deploy pipeline | | | Y / N / Partial |
| Live ops tools | | | Y / N / Partial |
| Economy/balance | | | Y / N / Partial |
| Art style/direction | | | Y / N / Partial |
| Platform relationships | | | Y / N / Partial |
| Analytics/data | | | Y / N / Partial |
| Player community | | | Y / N / Partial |
| Vendor relationships | | | Y / N / Partial |
| Key decision authority | | | Y / N / Partial |

### Step 2: Assess Each Key Person

| Person | Dependency Type | Area | Criticality (1-5) | Departure Risk (1-5) | Bus Factor Score |
|--------|-----------------|------|-------------------|---------------------|------------------|
| | Knowledge/Skill/Access/Capacity | | | | L×I = |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |

**Bus Factor Score** = Criticality × Departure Risk (higher = more urgent to address)

### Step 3: Mitigation Planning

For each high-scoring dependency:

| Person | Dependency | Mitigation Strategy | Owner | Target Date |
|--------|------------|---------------------|-------|-------------|
| | | ☐ Documentation ☐ Cross-training ☐ Redundancy ☐ Tooling | | |
| | | ☐ Documentation ☐ Cross-training ☐ Redundancy ☐ Tooling | | |
| | | ☐ Documentation ☐ Cross-training ☐ Redundancy ☐ Tooling | | |

## Framework: Mitigation Strategies

| Strategy | Best For | Investment | Effectiveness |
|----------|----------|------------|---------------|
| **Documentation** | Knowledge | Low-medium | Good for reference, poor for tacit knowledge |
| **Cross-training** | Skill, Knowledge | Medium-high | Effective but time-consuming |
| **Pair work** | Skill, Knowledge | Ongoing | Natural redundancy, slows immediate work |
| **Hiring redundancy** | Capacity, Skill | High | Most effective but expensive |
| **Tooling/Automation** | Knowledge, Skill | Variable | Encodes knowledge, reduces human dependency |
| **Process documentation** | Access, Knowledge | Low | Ensures others can follow steps |
| **Relationship introduction** | Access | Low | Builds backup relationships |

## Framework: Knowledge Documentation Priority

| Knowledge Type | Documentation Method | Priority Indicators |
|----------------|---------------------|---------------------|
| **Architecture decisions** | ADR (Architecture Decision Records) | Undocumented, complex, old |
| **System workflows** | Runbooks, playbooks | Operational, critical, repeated |
| **Historical context** | Wiki, decision log | Frequently asked, contentious |
| **Code quirks** | Code comments, README | Surprising behavior, workarounds |
| **Relationships** | Contact database, introduction emails | Single contact, important vendor |

## Framework: Cross-Training Plan Template

| Person Being Trained | Skill/Knowledge | Training From | Method | Hours Needed | Deadline | Status |
|---------------------|-----------------|---------------|--------|--------------|----------|--------|
| | | | Shadow / Pair / Course / Doc | | | |
| | | | | | | |
| | | | | | | |

## Framework: Departure Scenario Planning

For your top 3 key person dependencies:

**Scenario 1: [Person Name]**
- What they uniquely know/do: _______________
- If they left in 2 weeks:
  - Immediate impact: _______________
  - 30-day impact: _______________
  - Recovery plan: _______________
  - Recovery time estimate: _______________

**Scenario 2: [Person Name]**
- What they uniquely know/do: _______________
- If they left in 2 weeks:
  - Immediate impact: _______________
  - 30-day impact: _______________
  - Recovery plan: _______________
  - Recovery time estimate: _______________

**Scenario 3: [Person Name]**
- What they uniquely know/do: _______________
- If they left in 2 weeks:
  - Immediate impact: _______________
  - 30-day impact: _______________
  - Recovery plan: _______________
  - Recovery time estimate: _______________

## Checklist

- [ ] Critical areas identified
- [ ] Key person dependencies mapped
- [ ] Bus factor scores calculated
- [ ] Top 5 dependencies prioritized
- [ ] Mitigation strategy chosen for each
- [ ] Cross-training plan created
- [ ] Documentation backlog prioritized
- [ ] Departure scenarios considered

## Tasks

1. **List critical systems and areas** that would hurt if disrupted
2. **Identify the "hero" for each** — who do people go to?
3. **Score criticality and departure risk** honestly
4. **Pick top 3 to address** this quarter
5. **Start documentation** for highest-knowledge dependencies
6. **Schedule cross-training** for highest-skill dependencies
7. **Review quarterly** — dependencies shift as project evolves

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.4 Third-Party Risk Tracking

## Why It Matters

Modern games depend on dozens of third parties: SDKs for ads and analytics, platform services, cloud providers, outsourcing studios, middleware, and more. Each is a potential point of failure outside your control. When an ad SDK pushes a buggy update, when a platform changes its policies, when your outsource studio misses a deadline—your project suffers. Tracking these dependencies makes surprises manageable.

## Framework: Third-Party Dependency Inventory

```
┌─────────────────────────────────────────────────────────────────────┐
│                 THIRD-PARTY DEPENDENCY CATEGORIES                    │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  📱 PLATFORM                                                        │
│  ├── App Store (Apple, Google, Steam, console stores)               │
│  ├── Platform services (Game Center, Play Games, achievements)      │
│  ├── Platform payments (IAP systems)                                │
│  └── Certification/approval processes                               │
│                                                                     │
│  💰 MONETIZATION                                                    │
│  ├── Ad networks (mediation, individual networks)                   │
│  ├── Attribution (MMP)                                              │
│  ├── Payment processors                                             │
│  └── Offer walls, rewarded video providers                          │
│                                                                     │
│  📊 DATA & ANALYTICS                                                │
│  ├── Analytics platforms                                            │
│  ├── Crash reporting                                                │
│  ├── A/B testing services                                           │
│  └── Remote config services                                         │
│                                                                     │
│  ☁️ INFRASTRUCTURE                                                  │
│  ├── Cloud providers (AWS, GCP, Azure)                              │
│  ├── Backend services (PlayFab, GameSparks, Firebase)               │
│  ├── CDN providers                                                  │
│  └── Database services                                              │
│                                                                     │
│  🔧 TECHNOLOGY                                                      │
│  ├── Game engine (Unity, Unreal)                                    │
│  ├── Middleware (audio, physics, AI)                                │
│  ├── Third-party plugins and assets                                 │
│  └── Development tools and services                                 │
│                                                                     │
│  👥 SERVICES                                                        │
│  ├── Outsourcing studios (art, QA, porting)                         │
│  ├── Localization providers                                         │
│  ├── Customer support services                                      │
│  └── Marketing/UA agencies                                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Third-Party Risk Register

| Dependency | Category | Criticality | Risk Type | Risk Description | Mitigation | Owner |
|------------|----------|-------------|-----------|------------------|------------|-------|
| | Platform/Monetization/Data/Infra/Tech/Services | 1-5 | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |

### Risk Type Reference

| Risk Type | Description | Example |
|-----------|-------------|---------|
| **Policy change** | Terms, guidelines, requirements change | Apple changes IDFA rules |
| **Deprecation** | Service/API being retired | SDK end of life announcement |
| **Outage** | Service becomes unavailable | Cloud provider outage |
| **Quality** | Updates break things | SDK update causes crashes |
| **Pricing** | Cost changes | Cloud costs increase 3x |
| **Acquisition** | Company bought, priorities shift | Analytics company acquired |
| **Delivery** | Contracted work delayed/poor quality | Outsource studio misses deadline |

## Framework: Monitoring Approach by Category

| Category | What to Monitor | How | Frequency |
|----------|-----------------|-----|-----------|
| **Platform** | Policy updates, guideline changes | Developer blogs, newsletters | Weekly |
| **SDK/Monetization** | Release notes, deprecation notices | GitHub, vendor changelogs | Per release |
| **Infrastructure** | Status pages, incident history | Status page monitoring | Continuous |
| **Outsource** | Delivery cadence, quality trend | Milestone reviews | Per delivery |
| **Middleware** | Version support, roadmap | Vendor communication | Monthly |

## Framework: SDK Health Tracking

| SDK | Current Version | Latest Version | Last Updated | Update Urgency | Known Issues |
|-----|-----------------|----------------|--------------|----------------|--------------|
| | | | | Low/Medium/High/Critical | |
| | | | | | |
| | | | | | |
| | | | | | |

### SDK Update Decision Framework

| Condition | Action | Timeline |
|-----------|--------|----------|
| Security vulnerability | Update immediately | Days |
| Breaking change in latest | Evaluate, plan migration | 2-4 weeks |
| Minor update, no urgency | Bundle with next release | Next cycle |
| Major version, significant changes | Spike to assess effort, schedule | 1-3 months |
| Deprecation announced | Begin migration planning | Per vendor timeline |

## Framework: Outsource Vendor Risk Assessment

| Vendor | Service | Contract End | Criticality | Performance | Risk Level | Contingency |
|--------|---------|--------------|-------------|-------------|------------|-------------|
| | | | 1-5 | Red/Yellow/Green | | |
| | | | | | | |
| | | | | | | |

### Vendor Performance Indicators

| Indicator | Green | Yellow | Red |
|-----------|-------|--------|-----|
| On-time delivery | >90% | 70-90% | <70% |
| Quality (rework needed) | <10% | 10-30% | >30% |
| Communication | Proactive | Responsive | Delayed |
| Flexibility | Accommodating | Negotiable | Rigid |

## Framework: Platform Policy Tracking

| Platform | Policy Area | Current Rule | Last Changed | Risk of Change | Impact if Changed |
|----------|-------------|--------------|--------------|----------------|-------------------|
| Apple | IDFA/Privacy | | | | |
| Apple | IAP requirements | | | | |
| Google | Billing policy | | | | |
| Google | Privacy requirements | | | | |
| | | | | | |

## Framework: Contingency Planning

For your top 5 critical dependencies:

| Dependency | What If It Fails/Changes | Contingency Plan | Switch Cost (time/money) |
|------------|--------------------------|------------------|--------------------------|
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |

## Checklist

- [ ] All third-party dependencies inventoried
- [ ] Criticality scored for each
- [ ] Risk types identified
- [ ] Monitoring approach established
- [ ] SDK tracking in place
- [ ] Vendor performance tracked
- [ ] Platform policies monitored
- [ ] Contingency plans for critical dependencies

## Tasks

1. **Inventory all third parties** — often more than you think
2. **Categorize and score criticality** — which would hurt most?
3. **Set up monitoring** — status pages, newsletters, changelogs
4. **Create SDK tracking spreadsheet** with versions and dates
5. **Document contingencies** for top 5 critical dependencies
6. **Review quarterly** — add new dependencies, assess changes

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.5 Crunch Prevention Protocol

## Why It Matters

Crunch is often treated as inevitable in game development, but it's usually a failure of planning, process, or prioritization. Crunch burns out your best people, reduces code quality, damages morale, and creates technical debt that haunts you for years. Prevention requires structural safeguards built into the project from the start, not just good intentions.

## Framework: Crunch Warning Signs

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CRUNCH WARNING SYSTEM                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  🔴 RED FLAGS — Crunch is happening or imminent                     │
│  ├── Regular work exceeding 50 hours/week                           │
│  ├── Weekend work becoming expected, not exceptional                │
│  ├── "We just need to push through" becoming common phrase          │
│  ├── Sleep deprivation jokes in stand-ups                           │
│  ├── Morale visibly declining                                       │
│  └── Quality suffering despite more hours                           │
│                                                                     │
│  🟡 YELLOW FLAGS — Crunch trajectory forming                        │
│  ├── Buffer time being consumed                                     │
│  ├── Scope not adjusting as estimates grow                          │
│  ├── "Stretch goals" becoming expected                              │
│  ├── Hiring/resource requests denied despite overload               │
│  ├── Dependency delays not absorbed in plan                         │
│  └── "Just this once" becoming "just until milestone"               │
│                                                                     │
│  📊 QUANTITATIVE TRIGGERS                                            │
│  ├── Sprint velocity declining for 2+ sprints                       │
│  ├── Bug counts rising faster than declining                        │
│  ├── Overtime hours tracked exceeding threshold                     │
│  ├── PTO being canceled or not taken                                │
│  └── Sick days spiking                                              │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Root Causes of Crunch

| Root Cause | Warning Signs | Prevention |
|------------|---------------|------------|
| **Unrealistic deadline** | Deadline set before scope understood | Scope before date, or date before scope—not both |
| **Scope creep** | Features added without timeline adjustment | Formal change control, trade-offs required |
| **Estimation failure** | Estimates routinely exceeded | Reference-based estimates, contingency buffer |
| **Dependency delays** | External blockers compress internal schedule | Buffer for dependencies, early escalation |
| **Late-breaking requirements** | Major changes after production begins | Requirements freeze, change cost visibility |
| **Hero culture** | Overtime seen as dedication | Celebrate sustainable performance |
| **Communication failure** | Problems hidden until crisis | Psychological safety, early warning rewards |

## Framework: Structural Safeguards

| Safeguard | Implementation | Owner |
|-----------|----------------|-------|
| **Contingency buffer** | 15-20% schedule buffer built in | Producer |
| **Scope flexibility** | "Must have" vs "nice to have" explicit | Design lead |
| **Weekly hours tracking** | Visible team hours dashboard | Producer |
| **Overtime approval** | Manager approval required for >45 hours | All managers |
| **Mandatory PTO** | Minimum PTO days per quarter enforced | HR/Producer |
| **Scope/schedule trade-off** | Any scope add requires cut or delay | Product owner |
| **Early escalation** | Problems raised when 1 week behind, not 4 | All leads |
| **Retrospective action** | Crunch causes investigated and addressed | Team |

## Framework: Crunch Prevention Checklist by Phase

### Planning Phase

- [ ] Deadline set with input from people doing the work
- [ ] Scope explicitly tied to timeline and resources
- [ ] "Must have" vs "nice to have" documented
- [ ] 15-20% contingency built into schedule
- [ ] Dependencies identified with buffer
- [ ] Kill criteria established (what gets cut if behind)

### Production Phase

- [ ] Weekly hours visible and discussed
- [ ] Sprint velocity tracked
- [ ] Scope changes require formal approval
- [ ] Early warning threshold defined (when to escalate)
- [ ] PTO being taken, not deferred
- [ ] Buffer consumption tracked

### Pre-Milestone Phase

- [ ] Scope locked appropriately early
- [ ] "Feature complete" date honors integration time
- [ ] Bug fixing time protected
- [ ] Polish vs. feature trade-offs explicit
- [ ] Team health check conducted

## Framework: Intervention Protocol

When warning signs appear:

| Stage | Trigger | Response | Authority |
|-------|---------|----------|-----------|
| **Watch** | Yellow flags appearing | Discuss in team leads, monitor | Lead |
| **Alert** | Red flags appearing OR 45+ hour weeks | Escalate to director, review scope | Director |
| **Intervene** | Sustained 50+ hours OR health impacts | Cut scope, add resources, extend deadline | VP/Exec |
| **Emergency** | Team crisis, attrition, health incidents | Stop and reset | Executive |

## Framework: Conversation Templates

**For pushing back on unrealistic deadlines:**
> "To hit [date], we'd need [scope cut] or [additional resources]. Which would you prefer? Or if neither is acceptable, we need a different date."

**For escalating scope creep:**
> "This addition would require [X hours]. We can do it if we [cut Y] or [extend by Z]. What's the priority call?"

**For addressing crunch culture:**
> "I'm seeing [overtime pattern]. This is unsustainable and will hurt [quality/retention/health]. We need to [specific action] to fix the underlying cause."

## Framework: Your Project's Anti-Crunch Commitments

| Commitment | Threshold | Action if Breached | Owner |
|------------|-----------|-------------------|-------|
| Max sustained weekly hours | _____ hrs | | |
| Mandatory PTO per quarter | _____ days | | |
| Buffer before milestone | _____ weeks | | |
| Early warning trigger | | | |

## Checklist

- [ ] Warning signs documented and shared
- [ ] Root cause awareness trained
- [ ] Structural safeguards implemented
- [ ] Hours tracking in place
- [ ] Intervention protocol defined
- [ ] Leadership commitment secured
- [ ] Retrospectives investigate crunch causes
- [ ] Team educated on sustainable pace

## Tasks

1. **Share warning signs** with the team—everyone watches
2. **Implement hours tracking** (can be self-reported)
3. **Build contingency** into your current schedule
4. **Define your thresholds** — at what point do you escalate?
5. **Practice pushback conversations** — build the muscle
6. **Get leadership sign-off** on anti-crunch commitments

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.6 Retrospective Framework

## Why It Matters

Teams that don't retrospect repeat their mistakes. Retrospectives create structured time to reflect on what worked, what didn't, and what to try differently. But most retrospectives fail—they become venting sessions, generate actions that never happen, or are skipped when "too busy." A good framework makes retrospectives effective and efficient.

## Framework: Retrospective Types

| Type | When | Duration | Scope |
|------|------|----------|-------|
| **Sprint retro** | End of each sprint | 30-60 min | Last sprint only |
| **Milestone retro** | End of each milestone | 2-4 hours | Entire milestone |
| **Incident retro** | After significant incident | 1-2 hours | Specific incident |
| **Project retro** | End of project/launch | Half-day | Entire project |
| **Quarterly retro** | End of quarter | 2-3 hours | Quarter's work |

## Framework: Basic Retrospective Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                    RETROSPECTIVE FLOW                                │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  1. SET THE STAGE (5 min)                                           │
│     • Check-in, establish safety                                    │
│     • Remind of retrospective purpose                               │
│     • Review previous action items                                  │
│                                                                     │
│  2. GATHER DATA (15-20 min)                                         │
│     • What happened? (facts, not judgments)                         │
│     • What went well?                                               │
│     • What didn't go well?                                          │
│     • What surprised us?                                            │
│                                                                     │
│  3. GENERATE INSIGHTS (15-20 min)                                   │
│     • Why did things go well?                                       │
│     • Why did things go poorly?                                     │
│     • What patterns do we see?                                      │
│     • What's the root cause?                                        │
│                                                                     │
│  4. DECIDE WHAT TO DO (10-15 min)                                   │
│     • What experiments will we try?                                 │
│     • What will we stop doing?                                      │
│     • What will we start doing?                                     │
│     • Who owns each action?                                         │
│                                                                     │
│  5. CLOSE (5 min)                                                   │
│     • Summarize actions and owners                                  │
│     • Rate the retro                                                │
│     • Thank participants                                            │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Retrospective Techniques

### For Gathering Data

| Technique | How It Works | Best For |
|-----------|--------------|----------|
| **Start/Stop/Continue** | Three columns: what to start, stop, continue | Quick, familiar format |
| **Mad/Sad/Glad** | Emotional categorization of events | Teams that struggle to share feelings |
| **4 Ls** | Liked, Learned, Lacked, Longed for | Balanced positive/negative |
| **Timeline** | Plot events on a timeline, mark highs/lows | Longer periods, complex sprints |
| **Sailboat** | Wind (helps), anchor (slows), rocks (risks), island (goal) | Visual thinkers, remote teams |

### For Generating Insights

| Technique | How It Works | Best For |
|-----------|--------------|----------|
| **5 Whys** | Ask "why" repeatedly to find root cause | Single issue deep-dive |
| **Fishbone diagram** | Categorize causes by type | Complex problems |
| **Dot voting** | Vote on most important items | Prioritizing many items |
| **Patterns** | Look for recurring themes across items | Seeing systemic issues |

## Framework: Action Item Requirements

Every action item must have:

| Element | Description | Example |
|---------|-------------|---------|
| **Specific** | Clear, concrete action | "Add code review checklist" not "improve quality" |
| **Measurable** | Know when it's done | "Checklist created and posted" |
| **Owner** | Single person accountable | "Alex" not "the team" |
| **Deadline** | When it will be done | "By end of next sprint" |
| **Tracked** | Visible in shared system | In sprint backlog or action log |

## Framework: Action Item Tracking

| Action | Owner | Deadline | Status | Outcome |
|--------|-------|----------|--------|---------|
| | | | ☐ Planned ☐ In Progress ☐ Done ☐ Dropped | |
| | | | | |
| | | | | |
| | | | | |

**Action completion rate last 3 retros:** _______%

If completion rate <70%, you're generating too many actions or not prioritizing ruthlessly.

## Framework: Retrospective Anti-Patterns

| Anti-Pattern | Symptoms | Fix |
|--------------|----------|-----|
| **Venting session** | Complaining without action | Enforce insight and action phases |
| **Same issues every time** | Actions not completed or not effective | Track completion, try different solutions |
| **Silent participants** | Few people talk | Anonymous input, smaller groups, round-robin |
| **Blame game** | Individuals called out | Establish "blameless" norm, focus on systems |
| **Skipped when busy** | Retros canceled under pressure | Timebox strictly, make non-negotiable |
| **Too many actions** | Long lists, nothing gets done | Max 3 actions per retro |
| **No follow-through** | Actions generated but not tracked | Start next retro reviewing previous actions |

## Framework: Facilitator Checklist

Before:
- [ ] Book room/call, invite participants
- [ ] Choose technique appropriate for context
- [ ] Prepare materials (board, stickies, digital tool)
- [ ] Review previous retro actions

During:
- [ ] Start on time, end on time
- [ ] Establish psychological safety
- [ ] Ensure all voices heard
- [ ] Keep discussion constructive
- [ ] Drive toward specific actions
- [ ] Capture actions with owners and dates

After:
- [ ] Send summary and action items
- [ ] Add actions to tracking system
- [ ] Follow up on actions before next retro

## Framework: Your Retrospective Schedule

| Retro Type | Frequency | Duration | Facilitator | Participants |
|------------|-----------|----------|-------------|--------------|
| Sprint | | | | |
| Milestone | | | | |
| Quarterly | | | | |

## Checklist

- [ ] Retrospective cadence established
- [ ] Facilitator(s) identified and trained
- [ ] Technique library available
- [ ] Action tracking system in place
- [ ] Psychological safety norms established
- [ ] Retrospectives protected on calendar
- [ ] Previous actions reviewed at each retro
- [ ] Completion rate monitored

## Tasks

1. **Schedule your retro cadence** — put on calendar for the quarter
2. **Choose facilitator(s)** — rotating builds skill across team
3. **Select 2-3 techniques** to start with
4. **Create action tracking** in your existing system
5. **Run first retro** with explicit time for each phase
6. **Review action completion** at next retro

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.7 Post-Mortem Structure

## Why It Matters

Post-mortems are how organizations learn from failure. Without them, the same incidents happen repeatedly, eroding trust and burning out on-call teams. A good post-mortem is blameless, thorough, and action-oriented. It creates institutional memory that prevents future pain—but only if the process is followed consistently.

## Framework: Post-Mortem Principles

```
┌─────────────────────────────────────────────────────────────────────┐
│                    POST-MORTEM PRINCIPLES                            │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  1. BLAMELESS                                                       │
│     • Focus on systems and processes, not individuals               │
│     • People made decisions that seemed reasonable at the time      │
│     • "Who" is less important than "how" and "why"                  │
│     • Blame prevents honest discussion and future reporting         │
│                                                                     │
│  2. HONEST                                                          │
│     • Capture what actually happened, not the sanitized version     │
│     • Include uncomfortable truths                                  │
│     • Don't minimize impact or responsibility                       │
│     • Learning requires facing reality                              │
│                                                                     │
│  3. ACTIONABLE                                                      │
│     • Every post-mortem must produce specific action items          │
│     • Actions must have owners and deadlines                        │
│     • "Be more careful" is not an action                            │
│     • Systemic fixes preferred over procedural band-aids            │
│                                                                     │
│  4. TIMELY                                                          │
│     • Conduct within 48-72 hours while memory is fresh              │
│     • Don't wait for "more time to investigate"                     │
│     • Follow-up investigation can be an action item                 │
│                                                                     │
│  5. SHARED                                                          │
│     • Distribute learnings beyond the immediate team                │
│     • Similar incidents prevented elsewhere                         │
│     • Create organizational learning, not tribal knowledge          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Post-Mortem Template

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
POST-MORTEM: [Incident Title]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

METADATA
───────────────────────────────────────────────────────────────────────
Date:               [YYYY-MM-DD]
Severity:           [P0/P1/P2/P3]
Duration:           [Start time] - [End time] ([X hours/minutes])
Author:             [Name]
Participants:       [Names of people in post-mortem meeting]
Status:             [Draft / Final]

SUMMARY
───────────────────────────────────────────────────────────────────────
[2-3 sentence summary of what happened and impact]

IMPACT
───────────────────────────────────────────────────────────────────────
• Users affected:     [Number or percentage]
• Revenue impact:     [Estimated $]
• Duration:           [How long users were impacted]
• Other impacts:      [Reputation, support tickets, etc.]

TIMELINE (all times in [timezone])
───────────────────────────────────────────────────────────────────────
[HH:MM] - [What happened]
[HH:MM] - [What happened]
[HH:MM] - [What happened]
[HH:MM] - Incident detected by [how]
[HH:MM] - [Response action]
[HH:MM] - [Response action]
[HH:MM] - Incident resolved
[HH:MM] - Monitoring confirmed recovery

ROOT CAUSE
───────────────────────────────────────────────────────────────────────
[Clear explanation of the fundamental cause, not just the trigger]

CONTRIBUTING FACTORS
───────────────────────────────────────────────────────────────────────
• [Factor 1]
• [Factor 2]
• [Factor 3]

WHAT WENT WELL
───────────────────────────────────────────────────────────────────────
• [What helped contain or resolve the incident]
• [What worked in detection or response]
• [What prevented it from being worse]

WHAT WENT POORLY
───────────────────────────────────────────────────────────────────────
• [What extended or worsened the incident]
• [What was missing in detection or response]
• [What could have prevented this]

WHERE WE GOT LUCKY
───────────────────────────────────────────────────────────────────────
• [Things that could have made this much worse]
• [Coincidences that helped us]

ACTION ITEMS
───────────────────────────────────────────────────────────────────────
| Priority | Action | Owner | Deadline | Status |
|----------|--------|-------|----------|--------|
| P1 | | | | |
| P2 | | | | |
| P3 | | | | |

LESSONS LEARNED
───────────────────────────────────────────────────────────────────────
[Key insights for the organization]

APPENDIX
───────────────────────────────────────────────────────────────────────
[Links to logs, dashboards, Slack threads, support tickets, etc.]
```

## Framework: When to Write a Post-Mortem

| Trigger | Required Post-Mortem? | Notes |
|---------|----------------------|-------|
| P0/P1 incident | Yes, always | Within 48 hours |
| Revenue impact >$X | Yes | Define threshold for your business |
| User-facing outage >30 min | Yes | Adjust threshold as appropriate |
| Near-miss that could have been severe | Yes | Learn from close calls |
| P2 incident with interesting learnings | Recommended | Lighter-weight version OK |
| Recurring incident | Yes | Why is this happening again? |

## Framework: Root Cause Analysis

### The 5 Whys

Start with the incident and ask "why" repeatedly:

1. **Why** did the incident happen?
   - Answer: _______________

2. **Why** did that happen?
   - Answer: _______________

3. **Why** did that happen?
   - Answer: _______________

4. **Why** did that happen?
   - Answer: _______________

5. **Why** did that happen?
   - Answer: _______________

**Root cause identified:** _______________

### Common Root Cause Categories

| Category | Examples |
|----------|----------|
| **Process** | Missing checklist, unclear ownership, no review |
| **Technical** | Missing monitoring, inadequate testing, architectural weakness |
| **Communication** | Information not shared, unclear documentation |
| **Training** | Insufficient knowledge, unfamiliar systems |
| **Tooling** | Manual process error-prone, tools inadequate |
| **External** | Third-party failure, platform issue |

## Framework: Action Item Prioritization

| Priority | Definition | Timeline |
|----------|------------|----------|
| **P1** | Would prevent this specific incident from recurring | This sprint |
| **P2** | Would reduce likelihood or impact of similar incidents | This milestone |
| **P3** | Would improve detection or response capability | This quarter |

## Framework: Post-Mortem Meeting Agenda

| Phase | Duration | Purpose |
|-------|----------|---------|
| Set the stage | 5 min | Remind of blameless principle, state purpose |
| Review timeline | 10 min | Walk through what happened when |
| Identify causes | 15 min | 5 Whys, contributing factors |
| What went well/poorly | 10 min | Learn from both |
| Generate actions | 15 min | Specific, owned, prioritized |
| Wrap-up | 5 min | Assign document owner, set follow-up |

## Framework: Post-Mortem Review Meeting

| Question | Answer |
|----------|--------|
| Are all action items complete? | |
| Did the actions prevent recurrence? | |
| Have we seen similar incidents? | |
| Should we update the post-mortem? | |

## Checklist

- [ ] Post-mortem triggers defined
- [ ] Template created and accessible
- [ ] Blameless culture established
- [ ] Meeting process defined
- [ ] Action items tracked to completion
- [ ] Post-mortems shared broadly
- [ ] Review meeting scheduled for open items
- [ ] Post-mortem repository maintained

## Tasks

1. **Define your triggers** — what severity requires post-mortem?
2. **Customize the template** for your context
3. **Train the team** on blameless principles
4. **Run a practice post-mortem** on a recent issue
5. **Create a repository** for post-mortems
6. **Establish review cadence** for open action items

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6A.8 Decision Log

## Why It Matters

Six months from now, someone will ask "Why did we do it this way?" Without a decision log, the answer is lost—trapped in departed employees' heads, buried in old Slack threads, or simply forgotten. Decision logs preserve institutional knowledge, accelerate onboarding, prevent rehashing settled debates, and provide context when circumstances change.

## Framework: Decision Log Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                    DECISION LOG ENTRY                                │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  DECISION ID:       [Unique identifier]                             │
│  DATE:              [When decided]                                  │
│  DECISION:          [What was decided, stated clearly]              │
│  CONTEXT:           [What situation prompted this decision]         │
│  OPTIONS:           [What alternatives were considered]             │
│  RATIONALE:         [Why this option was chosen]                    │
│  CONSEQUENCES:      [Expected outcomes and trade-offs accepted]     │
│  DECIDERS:          [Who made or approved this decision]            │
│  STATUS:            [Active / Superseded / Revisit]                 │
│  REVISIT TRIGGER:   [Conditions that would warrant reconsidering]   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: What to Log

Log decisions that are:

| Criterion | Examples |
|-----------|----------|
| **Significant** | Architecture choices, feature cuts, business model decisions |
| **Contentious** | Decisions where team disagreed or stakeholders had strong opinions |
| **Irreversible** | Technology choices, platform commitments, major scope changes |
| **Recurring** | Questions that come up repeatedly—log once, reference forever |
| **Non-obvious** | Decisions that require explanation for future team members |

Don't log:
- Routine implementation choices
- Obvious decisions with clear answers
- Temporary decisions that will be revisited soon

## Framework: Decision Log Template

| ID | Date | Decision | Context | Options Considered | Rationale | Deciders | Status |
|----|------|----------|---------|-------------------|-----------|----------|--------|
| D001 | | | | | | | Active |
| D002 | | | | | | | Active |
| D003 | | | | | | | Active |
| D004 | | | | | | | Active |
| D005 | | | | | | | Active |

## Framework: Decision Categories

Organize your log by category for easier searching:

| Category | Examples |
|----------|----------|
| **Technical** | Engine choice, architecture patterns, infrastructure |
| **Design** | Core loop, monetization, target audience |
| **Scope** | Features cut, MVP definition, post-launch roadmap |
| **Process** | Sprint cadence, review processes, communication tools |
| **Business** | Platform priorities, pricing, market approach |
| **Team** | Hiring, org structure, vendor selection |

## Framework: Full Decision Entry Example

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
DECISION D042: Cut PvP Mode from Launch Scope
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Date: 2024-03-15
Status: Active
Category: Scope

DECISION
───────────────────────────────────────────────────────────────────────
PvP mode will not be included in v1.0 launch. It will be evaluated
for a post-launch update based on retention data.

CONTEXT
───────────────────────────────────────────────────────────────────────
Original scope included synchronous PvP mode. Schedule pressure and
technical complexity (netcode issues) created risk of 6+ week delay
to launch. Core loop validation showed strong single-player retention.

OPTIONS CONSIDERED
───────────────────────────────────────────────────────────────────────
1. Keep PvP, delay launch 6-8 weeks
2. Keep PvP, launch on time with known bugs
3. Cut PvP from launch, add in post-launch update
4. Cut PvP permanently, focus on PvE content

RATIONALE
───────────────────────────────────────────────────────────────────────
Option 3 chosen because:
- Launch window critical for UA timing (holiday season)
- Core loop validates without PvP
- PvP can be added post-launch without compromising single-player
- Option 2 would damage reviews and retention
- Option 4 premature—PvP may still have value

CONSEQUENCES ACCEPTED
───────────────────────────────────────────────────────────────────────
- Some player expectations may be disappointed
- Marketing messaging must avoid PvP references
- Technical work partially wasted (but learnings retained)
- Post-launch team must inherit PvP workstream

DECIDERS
───────────────────────────────────────────────────────────────────────
- [Game Director]: Recommended
- [Producer]: Recommended
- [VP Product]: Approved

REVISIT TRIGGER
───────────────────────────────────────────────────────────────────────
Revisit PvP priority if:
- D7 retention exceeds 35%
- Community requests exceed [threshold]
- Competitive landscape shifts to require PvP
```

## Framework: Decision Log Maintenance

| Task | Frequency | Owner |
|------|-----------|-------|
| Log significant decisions | As they happen | Decision maker |
| Review log for staleness | Monthly | Producer |
| Update superseded decisions | As superseded | Producer |
| Share with new team members | Onboarding | Manager |
| Archive completed project logs | End of project | Producer |

## Framework: Decision Search Aids

Make decisions findable:

| Search Method | How to Enable |
|---------------|---------------|
| **Tags/categories** | Apply consistent categories to each entry |
| **Keyword search** | Use consistent terminology in entries |
| **Date range** | All entries dated |
| **By decider** | Track who made each decision |
| **By status** | Active vs. superseded clearly marked |

## Framework: Connecting Decisions to Work

| Integration | How |
|-------------|-----|
| **Task/ticket reference** | Link from implementation tasks to decision ID |
| **Code comments** | Reference decision ID in relevant code |
| **Design docs** | Link to decision log for major choices |
| **Onboarding docs** | Include decision log as required reading |

## Checklist

- [ ] Decision log created and accessible
- [ ] Template established
- [ ] Categories defined
- [ ] Team knows when to log decisions
- [ ] Log reviewed regularly for staleness
- [ ] New team members shown decision log
- [ ] Log searchable/organized
- [ ] Connection to work items established

## Tasks

1. **Create your decision log** — wiki, spreadsheet, or doc
2. **Define what gets logged** — create guidelines for the team
3. **Seed with past decisions** — capture 5-10 significant past decisions
4. **Add logging to decision process** — make it a habit
5. **Include in onboarding** — new people read key decisions
6. **Review quarterly** — update status, archive stale entries

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# Track A Summary

## Risk Management Readiness Checklist

Before proceeding to Block 7A (Launch, Live Ops & Growth), confirm:

| Element | Complete? | Key Output |
|---------|-----------|------------|
| Risk Register — Development | | Register document with 15-25 risks |
| Likelihood × Impact Matrix | | Visual risk map, response strategies |
| Key Person Dependency Mapping | | Dependency audit, mitigation plan |
| Third-Party Risk Tracking | | Vendor inventory, monitoring approach |
| Crunch Prevention Protocol | | Safeguards, warning signs, thresholds |
| Retrospective Framework | | Cadence, technique, action tracking |
| Post-Mortem Structure | | Template, triggers, blameless culture |
| Decision Log | | Log structure, initial entries |

## Key Outputs from Block 6A

| Output | Location | Owner |
|--------|----------|-------|
| Development risk register | | |
| Risk matrix visualization | | |
| Key person mitigation plan | | |
| Third-party inventory | | |
| Anti-crunch commitments | | |
| Retrospective schedule | | |
| Post-mortem template | | |
| Decision log | | |

## Red Flags Requiring Attention

- [ ] No risk register exists
- [ ] Risks not reviewed for 4+ weeks
- [ ] Multiple single points of failure with no mitigation
- [ ] Third-party dependencies unknown or unmonitored
- [ ] Sustained overtime with no intervention
- [ ] Retrospectives skipped or ineffective
- [ ] Incidents repeat without post-mortem
- [ ] Decision rationale lost when people leave
