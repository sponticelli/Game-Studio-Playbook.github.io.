---
layout: default
title: "Scope and Change Management"
---

# Scope & Change Management

> *"The enemy of a good plan is the dream of a perfect plan."*  
> — Carl von Clausewitz

---

# Scope & Change Management (Greenfield Projects)

Complete these topics before entering production. Return to them when scope pressure mounts or change requests overwhelm the plan.

---

# 5A.1 Scope Creep Detection — Features

## Why It Matters

Scope creep is death by a thousand paper cuts. No single addition kills the project—each one seems reasonable in isolation. But they compound invisibly until the schedule is fiction, the team is demoralized, and the original vision is buried under accretions. Detecting scope creep requires explicit patterns and early warning systems, because by the time it's obvious, it's too late.

## Framework: Scope Creep Warning Signs

```
┌─────────────────────────────────────────────────────────────────────┐
│                    SCOPE CREEP WARNING SYSTEM                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ⚠️ VERBAL TRIGGERS — phrases that often precede scope creep        │
│  ├── "While we're at it..."                                         │
│  ├── "It would only take a few hours..."                            │
│  ├── "The competitor just shipped this..."                          │
│  ├── "What if we also..."                                           │
│  ├── "Can we just add..."                                           │
│  ├── "It's a quick win..."                                          │
│  ├── "Players will expect..."                                       │
│  └── "Since we're touching that code anyway..."                     │
│                                                                     │
│  📊 QUANTITATIVE SIGNALS                                             │
│  ├── Story points/hours added mid-sprint                            │
│  ├── Feature specs growing after approval                           │
│  ├── "v1.5" appearing between v1.0 and v2.0                         │
│  ├── Original estimates repeatedly exceeded                          │
│  ├── Dependencies multiplying faster than resolving                 │
│  └── "Final" reviews happening 3+ times                             │
│                                                                     │
│  🔍 BEHAVIORAL PATTERNS                                              │
│  ├── Design docs never quite finalized                              │
│  ├── Stakeholders adding feedback loops                             │
│  ├── "One more thing" at end of meetings                            │
│  ├── Features becoming "more strategic" mid-development             │
│  └── Scope discussions becoming emotional                           │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Scope Change Tracking

### Weekly Scope Delta Report

| Date | Feature | Change Type | Source | Impact (days) | Approved? |
|------|---------|-------------|--------|---------------|-----------|
| | | Added/Expanded/Modified | Who asked | | Y/N |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |

**Running totals:**
- Total scope additions this week: _______
- Total impact this week: _______ days
- Scope additions YTD: _______
- Total impact YTD: _______ days

## Framework: Creep vs. Legitimate Change

| Characteristic | Scope Creep | Legitimate Change |
|----------------|-------------|-------------------|
| **Trigger** | "Nice to have" | Data/research finding |
| **Documentation** | Informal request | Written proposal with impact |
| **Impact assessment** | "Shouldn't be too hard" | Engineering estimate provided |
| **Trade-off discussion** | None—additive only | Something removed or deferred |
| **Approval level** | Anyone says yes | Proper authority approves |
| **Timeline adjustment** | Schedule unchanged | Timeline revised if needed |

## Framework: Common Creep Vectors

| Source | How It Appears | Defense |
|--------|----------------|---------|
| **Stakeholder pressure** | "Leadership wants..." | Require formal request + impact |
| **Engineering gold-plating** | "While I'm in there..." | Scope PR reviews |
| **Design perfectionism** | "One more iteration..." | Time-box design phases |
| **QA discoveries** | "We should also test..." | Separate bugs from features |
| **Competitive reaction** | "X just launched Y..." | Evaluate against pillars |
| **Player requests** | "The community wants..." | Backlog, not roadmap |

## Framework: Scope Creep Severity Levels

| Level | Definition | Response |
|-------|------------|----------|
| **Level 1** | Minor addition, <1 day | Track, can be absorbed |
| **Level 2** | Medium addition, 1-5 days | Requires approval, may need trade-off |
| **Level 3** | Significant expansion, 1-2 weeks | Formal review, definite trade-off |
| **Level 4** | Major addition, >2 weeks | Milestone re-planning required |
| **Level 5** | Scope redefinition | Project reset or pivot discussion |

## Framework: Your Project's Scope Baseline

Document your baseline to detect drift:

| Feature | Scope Baseline | Current State | Drift |
|---------|---------------|---------------|-------|
| | Original definition | Current definition | +/- |
| | | | |
| | | | |
| | | | |
| | | | |

**Total baseline (story points/hours):** _______________

**Current total:** _______________

**Drift percentage:** _______________%

## Checklist

- [ ] Scope baseline documented for all major features
- [ ] Warning sign vocabulary shared with team
- [ ] Weekly scope delta tracking established
- [ ] Creep vs. legitimate change criteria defined
- [ ] Severity levels calibrated for your project
- [ ] Someone owns scope creep monitoring
- [ ] Regular scope health review scheduled

## Tasks

1. **Document your scope baseline** for current milestone
2. **Train team on trigger phrases** to recognize
3. **Establish weekly scope delta report** and owner
4. **Review last month's changes** — how many were creep?
5. **Post warning signs** where scope discussions happen

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.2 Scope Creep Detection — Live Ops

## Why It Matters

Live ops scope creep is sneakier than feature creep because it happens in operational rhythm rather than big decisions. Each event gets slightly more elaborate. Each sale requires more configuration. Each content update demands more assets. Before you know it, the "sustainable cadence" requires heroic effort, and the team burns out or quality collapses.

## Framework: Live Ops Creep Patterns

```
┌─────────────────────────────────────────────────────────────────────┐
│                  LIVE OPS SCOPE CREEP PATTERNS                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  📈 COMPLEXITY INFLATION                                             │
│  • Events that used to take 2 days now take 5 days                  │
│  • "Standard" templates keep getting customizations                 │
│  • Each event needs "just one more" unique element                  │
│  • Config files growing larger each cycle                           │
│                                                                     │
│  🏃 VELOCITY PRESSURE                                                │
│  • Monthly events become bi-weekly                                  │
│  • "One-time" events become recurring expectations                  │
│  • Content refresh rate keeps increasing                            │
│  • Players/stakeholders expect "always more"                        │
│                                                                     │
│  🛠️ TOOL DEBT ACCUMULATION                                           │
│  • Workarounds become permanent                                     │
│  • Manual processes multiply                                        │
│  • Same bugs get worked around repeatedly                           │
│  • Tool improvements constantly deprioritized                       │
│                                                                     │
│  👥 COMMUNICATION BURDEN                                             │
│  • More meetings needed per event                                   │
│  • Sign-off chains growing longer                                   │
│  • Documentation requirements expanding                             │
│  • Stakeholder reviews multiplying                                  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Live Ops Complexity Tracking

### Event Complexity Trend

| Event Name | Date | Prep Time | Team Hours | Assets | Configs | Bugs | Complexity Score |
|------------|------|-----------|------------|--------|---------|------|------------------|
| | | Days | Total | Count | Count | Post-launch | Sum |
| | | | | | | | |
| | | | | | | | |
| | | | | | | | |

**Trend direction:** ⬆️ Increasing / ➡️ Stable / ⬇️ Decreasing

## Framework: Sustainable Velocity Definition

Define what's sustainable BEFORE you launch:

| Metric | Sustainable Target | Current Reality | Gap |
|--------|-------------------|-----------------|-----|
| Events per month | | | |
| Content drops per month | | | |
| Offers/sales per month | | | |
| Config changes per week | | | |
| Average prep time per event | | | |
| Max team hours per week | | | |
| Overtime frequency | | | |

## Framework: Creep Triggers in Live Ops

| Trigger | Example | Healthy Response |
|---------|---------|------------------|
| **Success creates expectations** | "That event did great, let's do more!" | Define sustainable success rate |
| **Player requests** | "Players want weekly events" | Validate with data, not volume |
| **Competitor pressure** | "Rival ships content daily" | Compete on quality, not quantity |
| **Revenue targets** | "We need more sales events" | Measure per-event efficiency |
| **Stakeholder requests** | "Marketing wants themed events" | Add to backlog, evaluate capacity |
| **Team enthusiasm** | "We could make this so much cooler" | Time-box polish, preserve velocity |

## Framework: Live Ops Scope Boundaries

| Boundary Type | Definition | Your Limit |
|---------------|------------|------------|
| **Event ceiling** | Max events per month | |
| **Complexity cap** | Max prep days per event | |
| **Asset budget** | Max new assets per event | |
| **Config limit** | Max config changes per release | |
| **Team capacity** | Max hours per week for live ops | |
| **Overtime threshold** | Max overtime hours per quarter | |

## Framework: Creep Prevention Mechanisms

| Mechanism | Purpose | Implementation |
|-----------|---------|----------------|
| **Template enforcement** | Prevent one-off complexity | Events must use approved templates |
| **Complexity budget** | Cap elaboration | Fixed "complexity points" per event |
| **Velocity guard rails** | Prevent acceleration | Hard cap on events per month |
| **Pre-mortem for escalation** | Catch before commitment | "If we add this, what suffers?" |
| **Retrospective questions** | Catch after the fact | "What took longer than expected?" |

## Checklist

- [ ] Live ops baseline complexity documented
- [ ] Sustainable velocity targets defined
- [ ] Complexity tracking established
- [ ] Scope boundaries written and shared
- [ ] Prevention mechanisms in place
- [ ] Regular trend review scheduled
- [ ] Escalation path for boundary violations

## Tasks

1. **Calculate baseline complexity** for your last 5 events
2. **Define sustainable velocity** with your team
3. **Set explicit boundaries** for each metric
4. **Create complexity tracking** report
5. **Schedule monthly trend review**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.3 Feature Request Intake Process

## Why It Matters

Without a structured intake process, feature requests come from everywhere, in every format, with every level of urgency. The loudest voice wins. The person who catches you in the hallway gets their feature prioritized. Good ideas die in email threads while mediocre ideas with champions ship. A formal intake process creates fairness, visibility, and better decisions.

## Framework: Intake Funnel

```
┌─────────────────────────────────────────────────────────────────────┐
│                    FEATURE REQUEST INTAKE FUNNEL                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │                     CAPTURE                                  │   │
│  │  All requests submitted in standard format to single        │   │
│  │  location. No verbal-only requests, no email threads.       │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│                              ▼                                      │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │                     TRIAGE                                   │   │
│  │  Weekly review: Is it complete? Does it align with          │   │
│  │  pillars? Is it a duplicate? Is it urgent?                  │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│               ┌──────────────┴──────────────┐                       │
│               ▼                              ▼                       │
│  ┌─────────────────────┐        ┌─────────────────────┐            │
│  │     BACKLOG         │        │     REJECTED        │            │
│  │  Awaiting           │        │  With rationale     │            │
│  │  prioritization     │        │  and feedback       │            │
│  └──────────┬──────────┘        └─────────────────────┘            │
│             │                                                       │
│             ▼                                                       │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │                   EVALUATION                                 │   │
│  │  Detailed impact assessment, engineering estimate,          │   │
│  │  prioritization scoring                                     │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│               ┌──────────────┴──────────────┐                       │
│               ▼                              ▼                       │
│  ┌─────────────────────┐        ┌─────────────────────┐            │
│  │     ROADMAP         │        │     PARKING LOT     │            │
│  │  Scheduled for      │        │  Good idea, wrong   │            │
│  │  development        │        │  time               │            │
│  └─────────────────────┘        └─────────────────────┘            │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Feature Request Template

**Required fields for submission:**

| Field | Description | Example |
|-------|-------------|---------|
| **Title** | Clear, descriptive name | "Guild Chat System" |
| **Requester** | Who's asking | Product Manager, Community |
| **Source** | Where did this come from? | Player feedback, data, stakeholder |
| **Problem Statement** | What problem does this solve? | "Players can't coordinate in-game" |
| **Proposed Solution** | High-level approach | "Text chat in guild menu" |
| **Success Metrics** | How do we measure success? | "50% of guilds using daily" |
| **Urgency** | Why now? | "Retention data shows drop-off" |
| **Pillar Alignment** | Which pillar does this serve? | "Social: Build lasting friendships" |

**Optional but valuable:**

| Field | Description |
|-------|-------------|
| **User Story** | As a [user], I want [feature] so that [benefit] |
| **Comparable Examples** | Games/apps that do this well |
| **Dependencies** | Known blockers or requirements |
| **Risks** | What could go wrong |
| **Rough Sizing** | S/M/L/XL if known |

## Framework: Intake Triage Criteria

### Gate 1: Completeness Check

| Criterion | Pass? |
|-----------|-------|
| All required fields filled | ☐ |
| Problem statement is clear | ☐ |
| Requester can be reached for questions | ☐ |
| Not a duplicate of existing request | ☐ |

→ If incomplete: Return to requester with specific questions

### Gate 2: Strategic Alignment

| Question | Answer | Pass? |
|----------|--------|-------|
| Does it align with at least one pillar? | | ☐ |
| Does it support a current business goal? | | ☐ |
| Is it within our technical constraints? | | ☐ |
| Does it fit our target audience? | | ☐ |

→ If misaligned: Reject with clear rationale

### Gate 3: Timing Check

| Question | Answer |
|----------|--------|
| Is this needed before launch? | |
| Is there a time-sensitive opportunity? | |
| Are dependencies in place? | |
| Does team have capacity to evaluate? | |

→ Route to appropriate track (immediate, backlog, parking lot)

## Framework: Request Sources & Handling

| Source | Weight | Process |
|--------|--------|---------|
| **Player feedback (volume)** | High signal | Aggregate before acting |
| **Player feedback (individual)** | Low signal | Pattern matching only |
| **Data/analytics** | High signal | Validate and prioritize |
| **Stakeholder request** | Varies | Full intake process |
| **Team member idea** | Medium signal | Full intake process |
| **Competitive pressure** | Low signal | Evaluate against pillars |
| **Partner/platform requirement** | Mandatory if true | Verify and scope |

## Framework: Triage Cadence

| Activity | Frequency | Participants | Output |
|----------|-----------|--------------|--------|
| Intake review | Weekly | Producer + Lead | Triaged requests |
| Prioritization session | Bi-weekly | Core team | Updated backlog |
| Roadmap review | Monthly | Leadership | Roadmap decisions |
| Requester updates | Weekly | Producer | Status communications |

## Checklist

- [ ] Single submission location established
- [ ] Request template created and communicated
- [ ] Triage criteria defined
- [ ] Triage cadence scheduled
- [ ] Rejection process includes feedback
- [ ] Requester communication process defined
- [ ] Historical requests migrated to system

## Tasks

1. **Create submission form/template** in your project management tool
2. **Define triage meeting** cadence and participants
3. **Communicate intake process** to all stakeholders
4. **Process existing backlog** through new system
5. **Close the back door** — redirect ad-hoc requests

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.4 Change Impact Assessment

## Why It Matters

Every change ripples. A "simple" economy tweak affects progression, monetization, event design, and player sentiment. A UI change touches tutorials, localization, accessibility, and QA matrices. Without systematic impact assessment, teams underestimate work, miss dependencies, and create cascading problems. Impact assessment makes the true cost visible before commitment.

## Framework: Impact Dimensions

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CHANGE IMPACT DIMENSIONS                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                         ┌───────────────┐                           │
│                         │    CHANGE     │                           │
│                         │   PROPOSED    │                           │
│                         └───────┬───────┘                           │
│                                 │                                   │
│         ┌───────────────────────┼───────────────────────┐           │
│         │           │           │           │           │           │
│         ▼           ▼           ▼           ▼           ▼           │
│    ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐     │
│    │ DESIGN  │ │  TECH   │ │ECONOMY  │ │CONTENT  │ │TIMELINE │     │
│    │         │ │         │ │         │ │         │ │         │     │
│    │Systems  │ │Code     │ │Balance  │ │Assets   │ │Schedule │     │
│    │Balance  │ │Perf     │ │Monetize │ │Local    │ │Deps     │     │
│    │UX       │ │Infra    │ │Live     │ │QA       │ │Capacity │     │
│    └─────────┘ └─────────┘ └─────────┘ └─────────┘ └─────────┘     │
│         │           │           │           │           │           │
│         └───────────┴───────────┴───────────┴───────────┘           │
│                                 │                                   │
│                                 ▼                                   │
│                      ┌───────────────────┐                          │
│                      │   TOTAL IMPACT    │                          │
│                      │   ASSESSMENT      │                          │
│                      └───────────────────┘                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Impact Assessment Template

### Change Summary

| Field | Entry |
|-------|-------|
| Change Title | |
| Requester | |
| Date | |
| Assessor | |

### Design Impact

| Area | Affected? | Details | Effort |
|------|-----------|---------|--------|
| Core gameplay loop | Y/N | | |
| Progression systems | Y/N | | |
| Difficulty/balance | Y/N | | |
| Tutorial/onboarding | Y/N | | |
| UI/UX flows | Y/N | | |
| Player psychology | Y/N | | |

### Technical Impact

| Area | Affected? | Details | Effort |
|------|-----------|---------|--------|
| Client code | Y/N | | |
| Server code | Y/N | | |
| Database schema | Y/N | | |
| Build/deploy | Y/N | | |
| Performance | Y/N | | |
| Platform-specific | Y/N | | |
| SDK/middleware | Y/N | | |

### Economy Impact

| Area | Affected? | Details | Effort |
|------|-----------|---------|--------|
| Currency balance | Y/N | | |
| Pricing | Y/N | | |
| Reward structures | Y/N | | |
| Monetization touchpoints | Y/N | | |
| Live offers/events | Y/N | | |
| Historical player balances | Y/N | | |

### Content Impact

| Area | Affected? | Details | Effort |
|------|-----------|---------|--------|
| Art assets | Y/N | | |
| Audio assets | Y/N | | |
| Animation | Y/N | | |
| VFX | Y/N | | |
| Localization | Y/N | | |
| Store assets | Y/N | | |

### Timeline Impact

| Area | Affected? | Details | Impact |
|------|-----------|---------|--------|
| Current sprint | Y/N | | +___ days |
| Milestone date | Y/N | | +___ days |
| Launch date | Y/N | | +___ days |
| Dependencies | Y/N | List: | |
| Other features | Y/N | List: | |

### Summary

| Metric | Value |
|--------|-------|
| **Total effort (days)** | |
| **Total timeline impact** | |
| **Risk level** | Low / Medium / High |
| **Recommendation** | Proceed / Proceed with trade-offs / Defer / Reject |

## Framework: Impact Assessment Questions

| Category | Key Questions |
|----------|---------------|
| **Dependencies** | What has to happen before this? What does this block? |
| **Rework** | What existing work becomes invalid? |
| **Testing** | What needs retesting? New test cases needed? |
| **Documentation** | What docs need updating? |
| **Training** | Who needs to learn new things? |
| **Support** | What support issues might this create? |
| **Rollback** | Can we undo this if needed? |

## Framework: Second-Order Effects Checklist

Don't stop at first-order impact. Ask:

| First Order | → Second Order | → Third Order |
|-------------|----------------|---------------|
| Change to reward rates | → Affects player progression | → Changes monetization funnel |
| New feature added | → Requires tutorial update | → Affects new player retention |
| UI element moved | → Breaks muscle memory | → Increases support tickets |
| Performance optimization | → Enables new feature | → Unlocks new content type |

**Your change's ripple effects:**

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

## Framework: Assessment Depth by Change Size

| Change Size | Assessment Depth | Participants | Time |
|-------------|------------------|--------------|------|
| Trivial (<1 day) | Quick check | Lead only | 5 min |
| Small (1-3 days) | Brief assessment | Lead + 1 expert | 15 min |
| Medium (1-2 weeks) | Standard template | Cross-functional | 30-60 min |
| Large (>2 weeks) | Full assessment + meeting | All stakeholders | Half-day |

## Checklist

- [ ] Impact assessment template created
- [ ] All dimensions covered (design, tech, economy, content, timeline)
- [ ] Second-order effects considered
- [ ] Assessment depth calibrated to change size
- [ ] Process integrated into change approval
- [ ] Historical assessments archived for learning

## Tasks

1. **Create impact assessment template** for your project
2. **Calibrate dimensions** to your specific concerns
3. **Run assessment** on a recent change as practice
4. **Integrate into approval workflow**
5. **Review past surprises** — what impact did we miss?

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.5 Cost of Change Visualization

## Why It Matters

Abstract costs don't drive decisions. "This adds two weeks" doesn't land like "This means we miss the holiday window" or "This means cutting the tutorial." Visualizing the true cost—in terms stakeholders care about—makes trade-offs tangible and decisions honest. When everyone sees what we're really trading, scope discussions become productive.

## Framework: Cost Translation Table

| Abstract Cost | Concrete Translation |
|---------------|---------------------|
| +2 weeks | "We slip past [date]" |
| +$50K | "That's [N] months of [resource]" |
| +3 engineer-weeks | "Feature X gets delayed" |
| +1 sprint | "Soft launch moves to [date]" |
| +20% scope | "We're now a [bigger] game than planned" |

## Framework: Trade-Off Visualization

```
┌─────────────────────────────────────────────────────────────────────┐
│                    TRADE-OFF DECISION BOARD                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  IF WE ADD: _________________________________________________       │
│                                                                     │
│  ┌─────────────────────┐         ┌─────────────────────────────┐   │
│  │     WE GAIN:        │         │       WE LOSE:              │   │
│  │                     │         │                             │   │
│  │  •                  │         │  •                          │   │
│  │  •                  │         │  •                          │   │
│  │  •                  │         │  •                          │   │
│  │                     │         │                             │   │
│  └─────────────────────┘         └─────────────────────────────┘   │
│                                                                     │
│  ┌─────────────────────┐         ┌─────────────────────────────┐   │
│  │  TIMELINE IMPACT:   │         │  BUDGET IMPACT:             │   │
│  │                     │         │                             │   │
│  │  Launch: ______     │         │  Dev: $_______              │   │
│  │  Soft launch: ____  │         │  Marketing: $_______        │   │
│  │  Beta: ______       │         │  Ongoing: $_______/mo       │   │
│  │                     │         │                             │   │
│  └─────────────────────┘         └─────────────────────────────┘   │
│                                                                     │
│  ┌──────────────────────────────────────────────────────────────┐  │
│  │  WHAT WE CAN'T DO IF WE DO THIS:                             │  │
│  │                                                              │  │
│  │  •                                                           │  │
│  │  •                                                           │  │
│  │  •                                                           │  │
│  └──────────────────────────────────────────────────────────────┘  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Stakeholder-Specific Cost Framing

Different stakeholders care about different costs. Translate for your audience:

| Stakeholder | Cares About | Frame Cost As |
|-------------|-------------|---------------|
| **Executive** | Timeline, budget, risk | "This moves launch from Q2 to Q3" |
| **Marketing** | Launch windows, features for campaigns | "This means no guild feature for UA messaging" |
| **Finance** | Revenue, burn rate | "This adds $X to cost before revenue" |
| **Engineering** | Technical debt, architecture | "This creates maintenance burden for Y years" |
| **Design** | Player experience, vision | "This compromises the [pillar] pillar" |
| **QA** | Coverage, stability | "This adds X test cases, Y risk areas" |

## Framework: Visual Cost Comparison

### Option Comparison Matrix

| Criterion | Option A: Do It | Option B: Defer | Option C: Minimal |
|-----------|-----------------|-----------------|-------------------|
| **Timeline impact** | | | |
| **Budget impact** | | | |
| **Team impact** | | | |
| **Quality impact** | | | |
| **Revenue impact** | | | |
| **Strategic value** | | | |
| **Risk** | | | |
| **TOTAL** | | | |

### Timeline Visualization

```
Original Plan:
[Alpha]────[Beta]────[Soft]────[Launch]────[Live Ops]
   ▲         ▲          ▲          ▲
  Mar       May        Jul        Sep

With Addition:
[Alpha]────[Beta]──────[Soft]────────[Launch]────[Live Ops]
   ▲         ▲            ▲              ▲
  Mar       May          Sep            Nov
                         ↑
                   Holiday window missed
```

## Framework: Cost of Delay Calculation

| Factor | Value |
|--------|-------|
| Monthly operating cost | $_______ |
| Monthly revenue opportunity cost | $_______ |
| Per-week delay cost | $_______ |
| Seasonal window value | $_______ |
| Competitor first-mover risk | _______ |

**This change delays launch by ___ weeks = $_______**

## Framework: Sunk Cost Visibility

When arguing against a change that invalidates existing work:

| Work Already Done | Hours Invested | Would Need to Redo? | Waste |
|-------------------|----------------|---------------------|-------|
| | | Y/N | hours |
| | | | |
| | | | |
| **TOTAL** | | | |

"This change means _____ hours of completed work becomes waste."

## Framework: Opportunity Cost Board

| If We Do This | We CAN'T Do |
|---------------|-------------|
| Feature X | Feature Y |
| | Feature Z |
| | Bug fix batch |
| | Tool improvement |
| | Tech debt reduction |

"Every feature we add pushes something else out. What matters more?"

## Checklist

- [ ] Trade-off visualization created for current decisions
- [ ] Stakeholder-specific cost framing prepared
- [ ] Timeline impact visually represented
- [ ] Opportunity costs explicitly listed
- [ ] Cost of delay calculated
- [ ] All costs translated to tangible terms

## Tasks

1. **Create trade-off board** for your most contentious scope decision
2. **Calculate cost of delay** for your project
3. **List opportunity costs** of top 3 proposed additions
4. **Present visualized costs** in next planning meeting
5. **Get feedback** on which translations resonate

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.6 Cut/Keep/Defer Framework

## Why It Matters

When scope pressure mounts, teams often make reactive, emotional decisions about what to cut. Political capital wins over project needs. The loudest advocate saves their feature. The framework provides a systematic, defensible process for triage that focuses on project success rather than personal attachment.

## Framework: Triage Decision Tree

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CUT/KEEP/DEFER DECISION TREE                      │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    ┌─────────────────────┐                          │
│                    │    FEATURE/ITEM     │                          │
│                    │    IN QUESTION      │                          │
│                    └──────────┬──────────┘                          │
│                               │                                     │
│              ┌────────────────┴────────────────┐                    │
│              │ Is it CORE to the game's value  │                    │
│              │ proposition (core loop, pillars)?│                   │
│              └────────────────┬────────────────┘                    │
│                      │                 │                            │
│                     YES               NO                            │
│                      │                 │                            │
│                      ▼                 ▼                            │
│              ┌──────────────┐  ┌──────────────────┐                 │
│              │    KEEP      │  │ Is it BLOCKING   │                 │
│              │  (Protect)   │  │ other work?      │                 │
│              └──────────────┘  └────────┬─────────┘                 │
│                                   │           │                     │
│                                  YES         NO                     │
│                                   │           │                     │
│                                   ▼           ▼                     │
│                          ┌───────────┐ ┌──────────────────┐        │
│                          │   KEEP    │ │ Can we SIMPLIFY  │        │
│                          │ (Unblock) │ │ significantly?   │        │
│                          └───────────┘ └────────┬─────────┘        │
│                                           │           │             │
│                                          YES         NO             │
│                                           │           │             │
│                                           ▼           ▼             │
│                                   ┌───────────┐ ┌─────────────┐    │
│                                   │  SIMPLIFY │ │ Does it ADD │    │
│                                   │  & KEEP   │ │ significant │    │
│                                   └───────────┘ │ value?      │    │
│                                                 └──────┬──────┘    │
│                                                   │         │      │
│                                                  YES       NO      │
│                                                   │         │      │
│                                                   ▼         ▼      │
│                                            ┌─────────┐ ┌───────┐   │
│                                            │  DEFER  │ │  CUT  │   │
│                                            └─────────┘ └───────┘   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Triage Scoring Matrix

Score each item 1-5 (5 = highest):

| Feature | Core Value | Player Impact | Revenue Impact | Effort | Dependencies | Risk | TOTAL |
|---------|-----------|---------------|----------------|--------|--------------|------|-------|
| | /5 | /5 | /5 | Inverse /5 | # blocked | Low/Med/High | |
| | | | | | | | |
| | | | | | | | |
| | | | | | | | |
| | | | | | | | |

**Scoring guidance:**
- **Core Value (5):** Essential to pillars = 5, Nice enhancement = 2, Unrelated = 1
- **Player Impact (5):** DAU-defining = 5, Retention helper = 3, Marginal = 1
- **Revenue Impact (5):** Direct monetization = 5, Enables spending = 3, None = 1
- **Effort (Inverse 5):** <1 week = 5, 1-2 weeks = 3, >1 month = 1
- **Dependencies:** Count features blocked by this

## Framework: Triage Decision Criteria

### CUT when:

| Signal | Why |
|--------|-----|
| Low on all value scores | Doesn't justify investment |
| High effort, low impact | Poor ROI |
| No clear owner/champion | Likely to fail anyway |
| Doesn't align with pillars | Off-strategy |
| Can be replicated post-launch | Not MVP-essential |

### KEEP when:

| Signal | Why |
|--------|-----|
| Core to primary value proposition | Can't ship without it |
| Blocks multiple other features | Critical path |
| Already mostly done | Sunk cost makes completion efficient |
| High player/revenue impact | Strategic value |
| Commitment already made externally | Breaking promises is costly |

### DEFER when:

| Signal | Why |
|--------|-----|
| Valuable but not launch-critical | Good candidate for v1.1 |
| Dependencies not ready | Can't do it well now anyway |
| Team capacity unavailable | Better to wait than rush |
| Market timing not right | Feature before its time |
| Learning needed first | Data from launch will inform design |

## Framework: Forced Ranking Exercise

When you need to cut X items, force rank everything:

| Rank | Feature | Rationale |
|------|---------|-----------|
| 1 (Most essential) | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |
| ... | | |
| N (Least essential) | | |

**Draw the line:** Items below rank ___ are cut/deferred.

## Framework: The "Lifeboat" Exercise

Imagine you can only ship 5 features. Which 5?

1. _______________________
2. _______________________
3. _______________________
4. _______________________
5. _______________________

Everything else must justify why it's as important as these.

## Framework: Cut Documentation

For each cut item, document:

| Field | Entry |
|-------|-------|
| Feature/Item | |
| Decision | Cut / Defer to ______ |
| Rationale | |
| Decision maker | |
| Date | |
| Communication plan | |
| Resurrection criteria | What would bring this back? |

## Checklist

- [ ] Triage criteria defined for your project
- [ ] Scoring matrix created
- [ ] Decision tree applied to current scope
- [ ] Cut list documented with rationale
- [ ] Defer list has target dates
- [ ] Stakeholders informed of decisions
- [ ] Process for appealing decisions exists

## Tasks

1. **Score all features** using triage matrix
2. **Run decision tree** on bottom 25%
3. **Document all cut/defer decisions** with rationale
4. **Communicate decisions** to stakeholders
5. **Update roadmap and timeline**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.7 Minimum Viable Scope Definition

## Why It Matters

When everything goes wrong—budget cut, timeline compressed, key person leaves—you need to know the irreducible core. Minimum Viable Scope (MVS) is your emergency plan: the smallest version that's still worth shipping. Defining it in advance prevents panic decisions and ensures the core value proposition survives any cuts.

## Framework: MVS Layers

```
┌─────────────────────────────────────────────────────────────────────┐
│                    MINIMUM VIABLE SCOPE LAYERS                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌───────────────────────────────────────────────────────────────┐ │
│  │                                                               │ │
│  │   ┌───────────────────────────────────────────────────────┐   │ │
│  │   │                                                       │   │ │
│  │   │   ┌───────────────────────────────────────────────┐   │   │ │
│  │   │   │                                               │   │   │ │
│  │   │   │          SURVIVAL CORE                        │   │   │ │
│  │   │   │   The absolute minimum to be playable         │   │   │ │
│  │   │   │   and deliver core fantasy. Ship this         │   │   │ │
│  │   │   │   if everything falls apart.                  │   │   │ │
│  │   │   │                                               │   │   │ │
│  │   │   └───────────────────────────────────────────────┘   │   │ │
│  │   │                                                       │   │ │
│  │   │              VIABLE MINIMUM                           │   │ │
│  │   │   Core + enough content/polish to not                 │   │ │
│  │   │   embarrass us. Launchable but constrained.           │   │ │
│  │   │                                                       │   │ │
│  │   └───────────────────────────────────────────────────────┘   │ │
│  │                                                               │ │
│  │                  TARGET SCOPE                                 │ │
│  │   Viable + quality of life, content depth,                    │ │
│  │   polish. What we're actually planning.                       │ │
│  │                                                               │ │
│  └───────────────────────────────────────────────────────────────┘ │
│                                                                     │
│                      ASPIRATIONAL                                   │
│   Target + nice-to-haves, stretch goals.                            │
│   Only if everything goes better than planned.                      │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Survival Core Definition

The absolute minimum. If we could only ship ONE thing, what would it be?

| Component | What's Included | What's Cut |
|-----------|-----------------|------------|
| **Core Loop** | | |
| **Content Volume** | | |
| **Monetization** | | |
| **Meta Systems** | | |
| **Social Features** | | |
| **Live Ops** | | |
| **Polish Level** | | |
| **Platform Support** | | |

**One-sentence survival core:**

```
_______________________________________________________________________________
```

## Framework: MVS Feature List

| Feature | Survival Core | Viable Min | Target | Aspirational |
|---------|--------------|------------|--------|--------------|
| | ✓/✗ | ✓/✗ | ✓/✗ | ✓/✗ |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: MVS Triggers

When do you invoke MVS? Define in advance:

| Trigger | Threshold | Action |
|---------|-----------|--------|
| Budget cut | >___% reduction | Move to Viable Minimum |
| Timeline compression | >___ weeks lost | Re-evaluate against Viable Min |
| Key person loss | ___ leaves | Assess impact against MVS |
| Technical crisis | ___ blocked for >___ weeks | Scope to Survival Core |
| Metrics failure (soft launch) | Retention below ___ | Pivot or narrow scope |

## Framework: MVS Validation Questions

| Question | Survival Core | Viable Minimum |
|----------|---------------|----------------|
| Can someone complete one satisfying session? | Must be Yes | Yes |
| Would anyone pay anything? | Maybe | Must be Yes |
| Would we be embarrassed to show this? | Probably | No |
| Can we learn what we need to learn? | Yes | Yes |
| Does it represent our vision? | Barely | Yes |
| Can we build to Target from here? | Yes | Yes |

## Framework: MVS Content Scaling

| Content Type | Survival Core | Viable Min | Target |
|--------------|---------------|------------|--------|
| Levels/stages | | | |
| Characters/units | | | |
| Items/equipment | | | |
| Events/modes | | | |
| Tutorials | | | |
| Languages | | | |

## Framework: MVS Communication

Who needs to know your MVS and when to invoke it?

| Stakeholder | What They Need to Know | When to Tell Them |
|-------------|----------------------|-------------------|
| Executive | MVS exists, trigger conditions | Up front |
| Team | Full MVS definition | Up front |
| Marketing | Messaging impact of each tier | Before commitment |
| Partners | Dependency implications | If triggered |

## Checklist

- [ ] Survival Core defined
- [ ] Viable Minimum scoped
- [ ] Target Scope explicit (vs. aspirational)
- [ ] All features mapped to tiers
- [ ] Trigger conditions defined
- [ ] Team aligned on MVS definition
- [ ] Stakeholders aware MVS exists

## Tasks

1. **Define Survival Core** — the irreducible minimum
2. **Define Viable Minimum** — launchable but constrained
3. **Map all features** to scope tiers
4. **Set triggers** for when to invoke MVS
5. **Communicate MVS** to team and stakeholders

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.8 "Nice to Have" Parking Lot

## Why It Matters

Good ideas are the enemy of shipping. Without a designated place for deferred items, they either clutter the backlog, get forgotten, or keep resurfacing in planning meetings. The Parking Lot acknowledges value without commitment, keeps conversations productive, and preserves ideas for when capacity exists.

## Framework: Parking Lot Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                    FEATURE PARKING LOT                               │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  PURPOSE: A holding area for valuable ideas that aren't             │
│  prioritized for current scope. Not rejected—just waiting.          │
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │                        ACTIVE ROADMAP                        │   │
│  │                   (Committed, scheduled)                     │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│                              │ Not prioritized                      │
│                              ▼                                      │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │                        PARKING LOT                           │   │
│  │                    (Valuable, not now)                       │   │
│  │                                                              │   │
│  │  • Reviewed periodically                                     │   │
│  │  • Promoted when capacity exists                             │   │
│  │  • Archived if no longer relevant                            │   │
│  │                                                              │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│                              │ No longer relevant                   │
│                              ▼                                      │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │                        ARCHIVE                               │   │
│  │                 (Not pursuing, documented)                   │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Parking Lot Entry Template

| Field | Entry |
|-------|-------|
| **Idea Name** | |
| **Requester** | |
| **Date Parked** | |
| **Brief Description** | |
| **Why Valuable** | |
| **Why Not Now** | |
| **Estimated Effort** | S / M / L / XL |
| **Dependencies** | |
| **Trigger to Revisit** | |
| **Review Date** | |

## Framework: Parking Lot Categories

| Category | Definition | Review Frequency |
|----------|------------|------------------|
| **Post-Launch** | Good for v1.1 or v1.2 | Monthly |
| **If Capacity** | Do if team finishes early | Sprint-by-sprint |
| **Market Dependent** | Waiting on external factors | Quarterly |
| **Learning Needed** | Need data before committing | After launch |
| **Nice Polish** | Quality of life improvements | Monthly |
| **Experimental** | Unproven concepts | Quarterly |

## Framework: Parking Lot Management

### Entry Criteria

| Question | If Yes |
|----------|--------|
| Does this align with pillars? | Can park |
| Has it been impact-assessed? | Can park |
| Is there a clear reason it's not prioritized? | Can park |
| Is it documented enough to pick up later? | Can park |

### Exit Criteria (Promotion to Roadmap)

| Trigger | Action |
|---------|--------|
| Capacity opens up | Evaluate top parking lot items |
| Launch completes | Review entire parking lot |
| Data validates need | Promote related items |
| Dependency resolved | Promote unblocked items |
| Strategic shift | Re-evaluate all parked items |

### Exit Criteria (Archive)

| Trigger | Action |
|---------|--------|
| >12 months parked with no revisit | Archive |
| Strategy changed, no longer aligns | Archive |
| Better solution found | Archive |
| Original requester left, no champion | Review, likely archive |

## Framework: Your Parking Lot

| # | Idea | Category | Parked | Review By | Status |
|---|------|----------|--------|-----------|--------|
| 1 | | | | | Active/Promoted/Archived |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |

## Framework: Parking Lot Review Cadence

| Activity | Frequency | Participants | Output |
|----------|-----------|--------------|--------|
| Quick scan | Weekly | Producer | Flag items for promotion |
| Category review | Monthly | Leads | Promote/archive decisions |
| Full parking lot review | Quarterly | Core team | Major re-prioritization |
| Post-launch review | After launch | All stakeholders | v1.1 planning input |

## Framework: Communicating "Parked"

How to tell someone their idea is parked without killing their enthusiasm:

**Good response template:**

> "This is a good idea that aligns with [pillar]. We're parking it because [specific reason]. We'll revisit it [when/trigger]. It's documented in our parking lot and you can track its status at [location]."

**What NOT to say:**

- "Maybe someday" (vague, dismissive)
- "We'll see" (non-committal)
- "Good idea!" [then ignore] (dishonest)
- "We're focusing on other things" (no context)

## Checklist

- [ ] Parking lot system established
- [ ] Entry template created
- [ ] Categories defined for your project
- [ ] Review cadence scheduled
- [ ] Entry/exit criteria clear
- [ ] Team knows how to add items
- [ ] Stakeholders know parking ≠ rejection

## Tasks

1. **Create parking lot** in your project management tool
2. **Migrate existing "someday" items** to parking lot
3. **Define review cadence** and add to calendar
4. **Communicate system** to stakeholders
5. **Practice the response** for parking conversations

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.9 Stakeholder Expectation Management

## Why It Matters

Scope changes damage trust. Stakeholders who expected Feature X feel betrayed when it disappears—even if the decision was right. Managing expectations isn't manipulation; it's honest communication that preserves relationships and credibility. Well-managed expectations survive scope changes; poorly managed ones create lasting resentment.

## Framework: Stakeholder Communication Matrix

```
┌─────────────────────────────────────────────────────────────────────┐
│                STAKEHOLDER COMMUNICATION MATRIX                      │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  HIGH INFLUENCE  ┌────────────────────┬────────────────────┐        │
│                  │                    │                    │        │
│                  │      MANAGE        │     PARTNER        │        │
│                  │      CLOSELY       │                    │        │
│                  │                    │                    │        │
│                  │ Frequent updates   │ Collaborative      │        │
│                  │ Early warnings     │ Joint decisions    │        │
│                  │ Private briefings  │ Shared ownership   │        │
│                  │                    │                    │        │
│                  ├────────────────────┼────────────────────┤        │
│                  │                    │                    │        │
│                  │      MONITOR       │      INFORM        │        │
│                  │                    │                    │        │
│                  │ Periodic updates   │ Regular updates    │        │
│                  │ Standard channels  │ Highlight impacts  │        │
│                  │ Escalate if needed │ Answer questions   │        │
│                  │                    │                    │        │
│  LOW INFLUENCE   └────────────────────┴────────────────────┘        │
│                     LOW INTEREST          HIGH INTEREST             │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Stakeholder Map

| Stakeholder | Interest Level | Influence Level | Strategy | Update Frequency |
|-------------|---------------|-----------------|----------|------------------|
| | High/Med/Low | High/Med/Low | Partner/Manage/Inform/Monitor | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Scope Change Communication Template

### Before Communication, Answer:

| Question | Answer |
|----------|--------|
| What specifically changed? | |
| Why did it change? | |
| What's the impact on this stakeholder? | |
| What doesn't change? | |
| What's the path forward? | |
| When will we revisit this? | |

### Communication Structure:

1. **Lead with context** — Remind of shared goals
2. **State the change** — Clear, no sugarcoating
3. **Explain why** — Reasoning, not just decision
4. **Acknowledge impact** — Show you understand their concern
5. **Share alternatives** — What we're doing instead
6. **Commit to next steps** — When they'll hear more

### Example Template:

> "I wanted to update you on [feature/scope item]. Based on [reason—data, timeline, priority shift], we're [change]. I know this affects [their concern], and that matters to us too. Instead, we're [alternative/mitigation]. We'll revisit this [timing]. I'm available to discuss further."

## Framework: Expectation Setting Techniques

| Technique | When to Use | How |
|-----------|-------------|-----|
| **Ranges, not points** | Estimates, dates | "Between X and Y" not "exactly X" |
| **Confidence levels** | Commitments | "High confidence / Medium / Low" |
| **Explicit assumptions** | Plans | "This assumes A, B, C" |
| **Regular updates** | Ongoing | Don't wait for bad news |
| **Document commitments** | Agreements | Written record of what was promised |
| **Early warnings** | Bad news coming | Signal before it's critical |

## Framework: Trust Bank Account

Think of stakeholder trust as a bank account:

| Deposits | Withdrawals |
|----------|-------------|
| Delivering what you promised | Scope cuts without notice |
| Proactive communication | Surprises |
| Honest estimates | Missed dates |
| Quick response to concerns | Defensive reactions |
| Acknowledging their perspective | Dismissing their input |
| Following through | Dropped commitments |

**Current balance with key stakeholders:**

| Stakeholder | Recent Deposits | Recent Withdrawals | Balance |
|-------------|-----------------|-------------------|---------|
| | | | Positive/Negative |
| | | | |
| | | | |

## Framework: Difficult Conversation Preparation

When you have to deliver bad news:

| Element | Preparation |
|---------|-------------|
| **Facts** | What exactly is changing/happened? |
| **Impact** | How does this affect them specifically? |
| **Reason** | Why is this the right decision? |
| **Empathy** | What's their likely reaction? |
| **Alternatives** | What can you offer instead? |
| **Timeline** | When will things improve? |
| **Action** | What do you need from them? |

## Framework: Scope Change Announcement Checklist

- [ ] Change documented clearly
- [ ] Rationale documented
- [ ] Impact by stakeholder assessed
- [ ] Communication order determined (who hears first?)
- [ ] Key stakeholders briefed privately before announcement
- [ ] FAQ prepared for common questions
- [ ] Follow-up scheduled
- [ ] Feedback channel open

## Checklist

- [ ] Stakeholder map created
- [ ] Communication strategy per stakeholder defined
- [ ] Communication templates prepared
- [ ] Trust account self-assessment completed
- [ ] Process for scope change announcements established
- [ ] Feedback mechanism in place

## Tasks

1. **Map all stakeholders** with interest/influence
2. **Define communication strategy** for each quadrant
3. **Create communication template** for scope changes
4. **Assess trust balance** with key stakeholders
5. **Practice a difficult conversation** with a peer

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.10 Version Scoping Strategy

## Why It Matters

Not everything needs to ship in v1.0. In fact, trying to ship everything in v1.0 is how projects fail. Version scoping creates a roadmap that acknowledges reality: launch small, learn, expand. It shifts arguments from "in or out" to "now or later," which is often easier to resolve and leads to better outcomes.

## Framework: Version Timeline

```
┌─────────────────────────────────────────────────────────────────────┐
│                    VERSION TIMELINE FRAMEWORK                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ v1.0 - LAUNCH                                                │   │
│  │                                                              │   │
│  │ Core loop, minimum viable content, essential monetization   │   │
│  │ Goal: Prove the game works, establish baseline metrics      │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│                              │ 4-6 weeks                            │
│                              ▼                                      │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ v1.1 - QUICK FOLLOW                                          │   │
│  │                                                              │   │
│  │ Critical feedback fixes, first QoL improvements, bug fixes  │   │
│  │ Goal: Respond to launch learnings, retain early adopters    │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│                              │ 6-8 weeks                            │
│                              ▼                                      │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ v1.2 - FIRST MAJOR UPDATE                                    │   │
│  │                                                              │   │
│  │ First significant content addition, feature expansion       │   │
│  │ Goal: Re-engage lapsed players, deepen engagement           │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                              │                                      │
│                              │ 2-3 months                           │
│                              ▼                                      │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ v2.0 - MAJOR EXPANSION                                       │   │
│  │                                                              │   │
│  │ Significant new systems, possibly premium expansion         │   │
│  │ Goal: Reinvigorate game, attract new audience               │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Version Scoping Matrix

| Feature | v1.0 | v1.1 | v1.2 | v2.0 | Never |
|---------|------|------|------|------|-------|
| | ✓/✗ | ✓/✗ | ✓/✗ | ✓/✗ | ✓/✗ |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |

## Framework: Version Scoping Criteria

### v1.0 Criteria (Must Have)

| Criterion | Meets? |
|-----------|--------|
| Essential to core loop | ☐ |
| Required for monetization to function | ☐ |
| Needed for first-session experience | ☐ |
| Platform/store requirement | ☐ |
| No acceptable workaround exists | ☐ |

### v1.1 Criteria (Quick Follow)

| Criterion | Meets? |
|-----------|--------|
| Addresses likely launch feedback | ☐ |
| Small enough to ship in 4-6 weeks | ☐ |
| Improves retention without major change | ☐ |
| Fixes known pain point | ☐ |
| Low risk, high quality-of-life | ☐ |

### v1.2+ Criteria (Can Wait)

| Criterion | Meets? |
|-----------|--------|
| Valuable but not launch-critical | ☐ |
| Benefits from launch learnings | ☐ |
| Requires foundation from v1.0 | ☐ |
| Marketing tentpole for UA | ☐ |
| Significant development investment | ☐ |

### "Never" Criteria

| Criterion | Meets? |
|-----------|--------|
| Doesn't align with pillars | ☐ |
| Requires fundamental architecture change | ☐ |
| Market has moved on | ☐ |
| Better served by different game | ☐ |
| Opportunity cost too high | ☐ |

## Framework: Version Planning Template

### v1.0: ________________ (Target Date: _________)

| Category | Scope |
|----------|-------|
| Core gameplay | |
| Content volume | |
| Monetization | |
| Meta systems | |
| Social features | |
| Live ops ready | |
| Platform support | |

### v1.1: ________________ (Target Date: _________)

| Priority | Feature | Rationale |
|----------|---------|-----------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |

### v1.2: ________________ (Target Date: _________)

| Priority | Feature | Rationale |
|----------|---------|-----------|
| 1 | | |
| 2 | | |
| 3 | | |

### v2.0 Vision: _________________________________________

## Framework: "Later, Not Never" Conversation

When moving something to a future version:

| Element | Message |
|---------|---------|
| **Validate** | "This is a good feature that supports [pillar]" |
| **Explain** | "We're scheduling it for v1.2 because [reason]" |
| **Commit** | "It's documented and on the roadmap for [date]" |
| **Differentiate** | "This isn't rejection—it's prioritization" |

## Framework: Version Scope Lock Dates

| Version | Scope Lock | Feature Complete | Release |
|---------|------------|------------------|---------|
| v1.0 | | | |
| v1.1 | | | |
| v1.2 | | | |

**Rule:** After scope lock, only bug fixes and critical issues. Features move to next version.

## Checklist

- [ ] Version timeline defined
- [ ] All features assigned to versions
- [ ] Version criteria documented
- [ ] Scope lock dates set
- [ ] Team aligned on version strategy
- [ ] Stakeholders understand version plan
- [ ] Roadmap visual created

## Tasks

1. **Define your version timeline** with target dates
2. **Assign all backlog items** to versions or "never"
3. **Create version criteria** for your project
4. **Communicate version strategy** to team
5. **Create visual roadmap** for stakeholders

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.11 Pivot vs. Persist Criteria

## Why It Matters

Soft launch data rarely says "keep going exactly as planned." It forces a decision: double down on the current direction (persist), make fundamental changes (pivot), or stop entirely (kill). Without pre-defined criteria, this decision becomes political, emotional, or endless. Clear criteria make the conversation productive and the decision defensible.

## Framework: Decision Matrix

```
┌─────────────────────────────────────────────────────────────────────┐
│                    PIVOT VS. PERSIST DECISION MATRIX                 │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                              ENGAGEMENT                             │
│                                                                     │
│                    │          HIGH          │                       │
│    ┌───────────────┼───────────────────────┐│                       │
│    │               │                       ││                       │
│    │   OPTIMIZE    │       PERSIST         ││                       │
│    │               │                       ││                       │
│    │  Core works,  │   Metrics validate    ││                       │
│ M  │  monetization │   direction. Scale    ││                       │
│ O  │  needs work   │   and polish.         ││                       │
│ N  │               │                       ││                       │
│ E  ├───────────────┼───────────────────────┤│                       │
│ T  │               │                       ││                       │
│ I  │    PIVOT      │    INVESTIGATE        ││                       │
│ Z  │               │                       ││                       │
│ A  │  Fundamental  │   Something's off.    ││                       │
│ T  │  rethink      │   Dig deeper before   ││                       │
│ I  │  required     │   deciding.           ││                       │
│ O  │               │                       ││                       │
│ N  │               │                       ││                       │
│    └───────────────┴───────────────────────┘│                       │
│                    │          LOW           │                       │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Pre-Defined Thresholds

Define these BEFORE soft launch so the decision is objective:

### Retention Thresholds

| Metric | Persist | Optimize | Pivot | Kill |
|--------|---------|----------|-------|------|
| D1 Retention | >___% | ___-___% | <___% | <___% |
| D7 Retention | >___% | ___-___% | <___% | <___% |
| D30 Retention | >___% | ___-___% | <___% | <___% |

### Monetization Thresholds

| Metric | Persist | Optimize | Pivot | Kill |
|--------|---------|----------|-------|------|
| Conversion Rate | >___% | ___-___% | <___% | <___% |
| ARPDAU | >$___ | $___ - $___ | <$___ | <$___ |
| Day 7 LTV | >$___ | $___ - $___ | <$___ | <$___ |

### Engagement Thresholds

| Metric | Persist | Optimize | Pivot | Kill |
|--------|---------|----------|-------|------|
| Avg Sessions/Day | >___ | ___-___ | <___ | <___ |
| Avg Session Length | >___min | ___-___min | <___min | <___min |
| Core Loop Completion | >___% | ___-___% | <___% | <___% |

## Framework: Pivot Types

| Pivot Type | When to Consider | Example |
|------------|------------------|---------|
| **Core loop pivot** | Retention terrible despite engagement | Change fundamental mechanic |
| **Meta pivot** | Core fun but no progression pull | Redesign progression systems |
| **Monetization pivot** | Engagement but no spend | Rethink value proposition |
| **Audience pivot** | Wrong audience for this core | Retarget with same game |
| **Platform pivot** | Better fit elsewhere | Mobile → PC or vice versa |
| **Scope pivot** | Too ambitious | Simplify dramatically |

## Framework: Pivot Decision Process

```
┌─────────────────────────────────────────────────────────────────────┐
│                    PIVOT DECISION PROCESS                            │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  1. ASSESS                                                          │
│     └── Gather all soft launch data                                │
│         └── Compare against pre-defined thresholds                 │
│                                                                     │
│  2. DIAGNOSE                                                        │
│     └── If below threshold, WHY?                                   │
│         └── Is the problem fixable within current direction?       │
│                                                                     │
│  3. GENERATE OPTIONS                                                │
│     └── List possible paths forward                                │
│         └── Persist / Optimize / Pivot Type X / Kill               │
│                                                                     │
│  4. EVALUATE OPTIONS                                                │
│     └── For each option:                                           │
│         └── Cost (time, money, morale)                             │
│         └── Likelihood of success                                  │
│         └── Time to validate                                       │
│                                                                     │
│  5. DECIDE                                                          │
│     └── Make call with authority                                   │
│         └── Document rationale                                     │
│                                                                     │
│  6. COMMIT                                                          │
│     └── Communicate to team                                        │
│         └── Update plans                                           │
│         └── Set new validation milestones                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Pivot Readiness Assessment

| Factor | Current State | Implications |
|--------|---------------|--------------|
| **Budget remaining** | | Can we afford to pivot? |
| **Team morale** | | Will they support a pivot? |
| **Stakeholder patience** | | Is there appetite for change? |
| **Time to next milestone** | | Do we have runway? |
| **Core asset reusability** | | What survives a pivot? |
| **Market window** | | Is timing still viable? |

## Framework: Persist/Optimize/Pivot/Kill Criteria

Define for YOUR project:

### PERSIST when:

```
_______________________________________________________________________________

_______________________________________________________________________________
```

### OPTIMIZE when:

```
_______________________________________________________________________________

_______________________________________________________________________________
```

### PIVOT when:

```
_______________________________________________________________________________

_______________________________________________________________________________
```

### KILL when:

```
_______________________________________________________________________________

_______________________________________________________________________________
```

## Checklist

- [ ] Retention thresholds defined
- [ ] Monetization thresholds defined
- [ ] Engagement thresholds defined
- [ ] Pivot types understood
- [ ] Decision process documented
- [ ] Decision authority clear
- [ ] Team prepared for possibility of pivot

## Tasks

1. **Set your thresholds** before soft launch
2. **Document decision criteria** in shared location
3. **Assign decision authority** for pivot calls
4. **Brief team** on pivot possibility
5. **Prepare stakeholders** for data-driven decision

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.12 Sunk Cost Conversations

## Why It Matters

"But we've already spent six months on this." This is the sunk cost fallacy in action—past investment influencing future decisions even when that investment is irrelevant to future outcomes. Killing features you've invested in is emotionally hard but sometimes necessary. A framework for these conversations separates rational analysis from emotional attachment.

## Framework: Sunk Cost Reality Check

```
┌─────────────────────────────────────────────────────────────────────┐
│                    SUNK COST REALITY CHECK                           │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  THE PAST:                          THE FUTURE:                     │
│  ┌────────────────────────┐        ┌────────────────────────┐      │
│  │                        │        │                        │      │
│  │  What we've spent:     │        │  What it will take     │      │
│  │                        │        │  to complete:          │      │
│  │  • $______             │   VS   │                        │      │
│  │  • ____ hours          │        │  • $______             │      │
│  │  • ____ months         │        │  • ____ hours          │      │
│  │                        │        │  • ____ months         │      │
│  │  CANNOT BE RECOVERED   │        │  STILL TO BE SPENT     │      │
│  │                        │        │                        │      │
│  └────────────────────────┘        └────────────────────────┘      │
│                                                                     │
│  THE QUESTION:                                                      │
│  ┌──────────────────────────────────────────────────────────────┐  │
│  │                                                              │  │
│  │  If we were starting fresh TODAY with the future cost,      │  │
│  │  would we choose to build this feature?                     │  │
│  │                                                              │  │
│  │  If NO → The sunk cost is making you irrational. Cut it.    │  │
│  │  If YES → Proceed, but verify it's not emotional.           │  │
│  │                                                              │  │
│  └──────────────────────────────────────────────────────────────┘  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Kill Decision Template

| Question | Answer |
|----------|--------|
| **Feature/System** | |
| **Already invested** | $___ / ___ hours / ___ months |
| **Remaining to complete** | $___ / ___ hours / ___ months |
| **If starting fresh, would we build this?** | Yes / No / Unsure |
| **What changes if we kill it?** | |
| **What do we gain by killing it?** | |
| **What do we lose by killing it?** | |
| **Is there a minimal viable version?** | |
| **Recommendation** | Kill / Reduce / Proceed |

## Framework: Arguments FOR Killing

Use these to counter sunk cost bias:

| Argument | How It Helps |
|----------|--------------|
| "The past investment is gone either way" | Reframes as forward-looking |
| "Completing it costs X more; is that worth it?" | Focuses on remaining investment |
| "What else could we do with those resources?" | Highlights opportunity cost |
| "Would we start this today?" | Tests true value |
| "Is our attachment emotional or rational?" | Names the bias |
| "A failed feature damages more than a missing one" | Considers downside |

## Framework: When to Kill vs. When to Reduce

| Kill When | Reduce When |
|-----------|-------------|
| Fundamental design flaw | Implementation issues only |
| No longer fits strategy | Still strategic, just oversized |
| No champion remaining | Passionate owner exists |
| Better alternatives emerged | Still best approach |
| Opportunity cost too high | Marginal cost to finish |
| Quality will always be poor | Quality achievable at smaller scale |

## Framework: The Conversation Structure

### 1. Set the Frame

> "I want to discuss whether [feature] is still the right investment. I know we've put a lot into it, and I want to make sure we're making this decision based on future value, not past investment."

### 2. Present the Data

> "Here's what we've invested: [past costs]. Here's what it would take to complete: [future costs]. Here's what we get: [expected value]."

### 3. Ask the Key Question

> "If we were starting today, knowing what we know now, would we choose to build this?"

### 4. Acknowledge Emotions

> "I know this is hard. We've all invested in this. But I want to make sure we're not continuing because we feel we have to."

### 5. Decide and Document

> "Based on this discussion, we're [decision]. Here's why: [rationale]."

## Framework: Salvage Assessment

Before killing, assess what can be salvaged:

| Component | Salvageable? | Reuse Opportunity |
|-----------|--------------|-------------------|
| Code/systems | | |
| Art assets | | |
| Design learnings | | |
| Technical learnings | | |
| Team skills developed | | |
| Documentation | | |

## Framework: Team Communication

When announcing a kill decision:

| Element | Message |
|---------|---------|
| **Acknowledge investment** | "I know everyone put a lot into this." |
| **Explain rationale** | "Here's why this is the right call." |
| **Honor the work** | "What we learned will help us on [X]." |
| **Focus forward** | "Here's where that energy goes now." |
| **Invite input** | "If you see this differently, let's discuss." |

## Framework: Personal Sunk Cost Check

Before advocating to keep something, ask yourself:

| Question | Answer |
|----------|--------|
| Did I personally invest heavily in this? | Y/N |
| Would I feel embarrassed if it's cut? | Y/N |
| Am I the primary champion? | Y/N |
| Is my identity tied to this? | Y/N |
| Am I avoiding admitting a mistake? | Y/N |

**If 3+ Yes answers:** Your judgment may be compromised by sunk cost. Seek outside perspective.

## Checklist

- [ ] Sunk cost concept understood by team
- [ ] Kill decision template created
- [ ] Salvage assessment process defined
- [ ] Communication approach prepared
- [ ] Team briefed on rational decision-making
- [ ] Personal bias check practiced

## Tasks

1. **Review current features** through sunk cost lens
2. **Practice the conversation** with a non-controversial example
3. **Create salvage inventory** for at-risk features
4. **Brief team** on sunk cost fallacy
5. **Document kill decisions** with full rationale

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.13 Scope Lock Protocol

## Why It Matters

Without a formal scope lock, features keep sneaking in until the day before launch. "Just one more thing" becomes "ten more things" and suddenly the release is at risk. Scope lock creates a clear line: before this date, changes are possible; after, only bug fixes. It protects the team's ability to deliver and forces prioritization earlier.

## Framework: Scope Lock Timeline

```
┌─────────────────────────────────────────────────────────────────────┐
│                    SCOPE LOCK TIMELINE                               │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ──────────────────────────────────────────────────────────────▶   │
│                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌──────────┐   │
│  │   SCOPE     │  │  FEATURE    │  │   CODE      │  │ RELEASE  │   │
│  │   OPEN      │──│  COMPLETE   │──│   FREEZE    │──│          │   │
│  │             │  │             │  │             │  │          │   │
│  │ Changes     │  │ No new      │  │ Bug fixes   │  │ Ship it  │   │
│  │ evaluated   │  │ features    │  │ only        │  │          │   │
│  │ normally    │  │ after this  │  │             │  │          │   │
│  └─────────────┘  └─────────────┘  └─────────────┘  └──────────┘   │
│                          ▲                ▲                         │
│                          │                │                         │
│                    SCOPE LOCK       CODE FREEZE                     │
│                    (Feature lock)   (Content lock)                  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Lock Types

| Lock Type | What It Means | What's Allowed | What's Not |
|-----------|---------------|----------------|------------|
| **Scope Lock** | No new features | Bug fixes, polish, tuning | Feature additions |
| **Content Lock** | No new content | Balance tuning, bug fixes | New levels, characters |
| **Code Freeze** | Minimal code changes | Critical bug fixes only | Any new code |
| **Config Freeze** | No config changes | Emergency fixes only | Any data changes |

## Framework: Scope Lock Dates

| Lock Type | Date | Days Before Release |
|-----------|------|---------------------|
| **Scope Lock** | | |
| **Content Lock** | | |
| **Code Freeze** | | |
| **Config Freeze** | | |
| **Release** | | 0 |

## Framework: Scope Lock Announcement

### Pre-Lock Countdown

| Timing | Action |
|--------|--------|
| 2 weeks before | Announce scope lock date, explain rules |
| 1 week before | Final scope review, last chance for changes |
| 3 days before | Lock warning, no non-critical changes |
| Lock day | Official lock, protocol in effect |

### Lock Announcement Template

> **SCOPE LOCK EFFECTIVE [DATE]**
>
> As of [date], we are in scope lock for [release]. This means:
>
> ✅ **Allowed:** Bug fixes, polish, tuning, documentation
> ❌ **Not allowed:** New features, scope changes, "just one more thing"
>
> Any exceptions require [approval authority] sign-off via the Post-Lock Exception Process.
>
> Next milestone: [Code Freeze on DATE]

## Framework: What's In vs. Out After Lock

| Category | ALLOWED | NOT ALLOWED |
|----------|---------|-------------|
| **Code** | Bug fixes | New features |
| **Art** | Polish, fixes | New assets |
| **Design** | Balance tuning | New mechanics |
| **Audio** | Level adjustments | New assets |
| **UI** | Bug fixes | New screens |
| **Content** | Fixes only | New levels, items |
| **Analytics** | Fixes | New instrumentation |

## Framework: Lock Enforcement

| Violation | Response |
|-----------|----------|
| Small change slipped in | Discuss with team, document, warn |
| Repeated violations | Escalate to leadership |
| Significant feature added | Revert change, formal post-mortem |
| Emergency exception claimed | Route through Post-Lock Exception Process |

## Framework: Lock Authority

| Decision | Authority |
|----------|-----------|
| Call scope lock | |
| Grant post-lock exception | |
| Override lock (emergency) | |
| Extend lock period | |

## Framework: Pre-Lock Checklist

Before declaring scope lock:

- [ ] All planned features implemented or formally deferred
- [ ] Feature list final and documented
- [ ] Known issues documented with severity
- [ ] Bug backlog triaged
- [ ] Team aware of lock date
- [ ] Stakeholders aligned on scope
- [ ] Exception process communicated
- [ ] Lock announcement prepared

## Framework: Post-Lock Rules of Engagement

| If Someone Asks... | Response |
|-------------------|----------|
| "Can we just add X real quick?" | "We're in scope lock. File an exception request." |
| "This is critical for [reason]" | "Use the exception process to document impact." |
| "It's tiny, no one will notice" | "All changes go through exception process." |
| "Leadership wants this" | "Leadership can approve an exception formally." |

## Checklist

- [ ] Lock types defined for your project
- [ ] Lock dates set and communicated
- [ ] Allowed vs. not allowed criteria clear
- [ ] Enforcement approach defined
- [ ] Authority assigned
- [ ] Team trained on lock protocol
- [ ] Exception process ready

## Tasks

1. **Set lock dates** for current milestone
2. **Define lock types** appropriate for your project
3. **Communicate lock schedule** to team and stakeholders
4. **Prepare enforcement** approach
5. **Test the process** with a mock scenario

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 5A.14 Post-Lock Exception Process

## Why It Matters

Scope lock without an exception process becomes either ignored or weaponized. Emergencies happen—critical bugs, platform requirements, revenue-impacting issues. The exception process provides a controlled valve for genuinely necessary changes while maintaining the discipline that lock provides. It's not a loophole; it's a formal, documented, accountable process.

## Framework: Exception Decision Tree

```
┌─────────────────────────────────────────────────────────────────────┐
│                    EXCEPTION DECISION TREE                           │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    ┌─────────────────────┐                          │
│                    │   CHANGE REQUESTED  │                          │
│                    │   AFTER SCOPE LOCK  │                          │
│                    └──────────┬──────────┘                          │
│                               │                                     │
│              ┌────────────────┴────────────────┐                    │
│              │ Is it a CRITICAL bug fix?       │                    │
│              │ (Crash, data loss, security)    │                    │
│              └────────────────┬────────────────┘                    │
│                      │                 │                            │
│                     YES               NO                            │
│                      │                 │                            │
│                      ▼                 ▼                            │
│              ┌──────────────┐  ┌────────────────────┐               │
│              │    FIX IT    │  │ Is it a PLATFORM   │               │
│              │  (Standard   │  │ REQUIREMENT?       │               │
│              │  bug process)│  │ (Store rejection)  │               │
│              └──────────────┘  └────────┬───────────┘               │
│                                   │           │                     │
│                                  YES         NO                     │
│                                   │           │                     │
│                                   ▼           ▼                     │
│                           ┌───────────┐ ┌──────────────────┐       │
│                           │  FIX IT   │ │ Is it REVENUE    │       │
│                           │(Must have)│ │ CRITICAL?        │       │
│                           └───────────┘ │ (>$X impact)     │       │
│                                         └────────┬─────────┘       │
│                                            │           │            │
│                                           YES         NO            │
│                                            │           │            │
│                                            ▼           ▼            │
│                                    ┌───────────┐ ┌──────────────┐  │
│                                    │ EXCEPTION │ │    DEFER     │  │
│                                    │ REQUEST   │ │  TO NEXT     │  │
│                                    │ REQUIRED  │ │  VERSION     │  │
│                                    └───────────┘ └──────────────┘  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Exception Request Template

| Field | Entry |
|-------|-------|
| **Requester** | |
| **Date** | |
| **Change Title** | |
| **Type** | Bug / Feature / Content / Config |
| **Urgency** | Critical / High / Medium |
| **Description** | What needs to change? |
| **Justification** | Why can't this wait? |
| **Impact if NOT done** | What happens if we defer? |
| **Impact if done** | Risk to release? |
| **Effort** | Hours to implement |
| **Testing required** | What needs retesting? |
| **Risk** | What could go wrong? |
| **Rollback plan** | How to undo if needed? |

## Framework: Exception Categories

| Category | Criteria | Typical Approval |
|----------|----------|------------------|
| **Critical Bug** | Crash, data loss, security, certification blocker | Lead approval, fast track |
| **Platform Requirement** | Store rejection, compliance | Auto-approve, document |
| **Revenue Impact** | >$X/day loss or >Y% conversion impact | Leadership approval |
| **Legal/Compliance** | Legal exposure, policy violation | Must fix, document |
| **User Experience** | Severe UX issue affecting reviews | Exception process |
| **Nice to Have** | Everything else | DENIED - defer to next version |

## Framework: Exception Approval Levels

| Exception Type | Approver | Escalation |
|----------------|----------|------------|
| Critical bug fix | Lead | Producer if disputed |
| Platform requirement | Producer | Director if timeline impact |
| Revenue impact | Director | VP if major |
| Legal/Compliance | Director + Legal | C-level if needed |
| Feature request | DENIED | Appeal to VP |

## Framework: Exception Process Workflow

```
1. Requester completes Exception Request Template
                    │
                    ▼
2. Impact assessment (Engineering, QA)
                    │
                    ▼
3. Review by appropriate approver (based on category)
                    │
         ┌─────────┴─────────┐
         │                   │
      APPROVED            DENIED
         │                   │
         ▼                   ▼
4. Implementation      Documented
   with tracking       with rationale
         │
         ▼
5. Verification and sign-off
         │
         ▼
6. Documentation in exception log
```

## Framework: Exception Log

| # | Date | Change | Category | Requester | Approver | Outcome | Impact |
|---|------|--------|----------|-----------|----------|---------|--------|
| 1 | | | | | | Approved/Denied | |
| 2 | | | | | | | |
| 3 | | | | | | | |
| 4 | | | | | | | |
| 5 | | | | | | | |

## Framework: Denied Exception Response

When denying an exception:

| Element | Message |
|---------|---------|
| **Acknowledge** | "I understand why this seems important." |
| **Explain** | "Here's why it doesn't meet exception criteria: [reason]" |
| **Alternative** | "This is scheduled for v1.1 / will be addressed post-launch" |
| **Commit** | "I've documented it and we'll revisit on [date]" |

## Framework: Exception Abuse Signs

Watch for patterns that indicate the process is being circumvented:

| Warning Sign | Response |
|--------------|----------|
| High volume of requests | Review lock discipline, retrain |
| Same requester repeatedly | Direct conversation |
| "Critical" used loosely | Tighten criteria definitions |
| Approvers always saying yes | Review approval standards |
| Requests coming late | Earlier lock communication |
| Political pressure to approve | Escalate to leadership |

## Framework: Post-Release Exception Review

After release, review all exceptions:

| Question | Finding |
|----------|---------|
| How many exceptions were granted? | |
| How many were truly necessary? | |
| Did any cause problems? | |
| Were any denied that shouldn't have been? | |
| What patterns emerged? | |
| How do we improve the process? | |

## Checklist

- [ ] Exception request template created
- [ ] Exception categories defined
- [ ] Approval levels assigned
- [ ] Process workflow documented
- [ ] Exception log established
- [ ] Team trained on when to request exceptions
- [ ] Approvers aligned on criteria
- [ ] Post-release review scheduled

## Tasks

1. **Create exception request template** in your tracking system
2. **Define exception categories** and criteria for your project
3. **Assign approvers** for each category
4. **Communicate process** to team
5. **Practice with a scenario** before lock

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```
