---
layout: default
title: "Team Structure for Live Ops (Mature Games)"
---

# Team Structure for Live Ops (Mature Games)

# 3B.1 Live Ops Team Structure Assessment

## Why It Matters

A team built for development is different from one built for live operations. Development needs broad capability; live ops needs consistent execution, rapid response, and sustainable pace. Assessing your current structure reveals gaps between what you have and what live ops requires.

## Framework: Live Ops Team Model

```
┌─────────────────────────────────────────────────────────────────────┐
│                    LIVE OPS TEAM STRUCTURE                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                      ┌───────────────────┐                          │
│                      │    LIVE OPS       │                          │
│                      │    LEAD           │                          │
│                      │ (Owns cadence,    │                          │
│                      │  calendar, health)│                          │
│                      └─────────┬─────────┘                          │
│                                │                                    │
│       ┌────────────────────────┼────────────────────────┐           │
│       │                        │                        │           │
│       ▼                        ▼                        ▼           │
│  ┌─────────────┐      ┌─────────────────┐      ┌─────────────┐     │
│  │   EVENT     │      │    CONTENT      │      │   ECONOMY   │     │
│  │   TEAM      │      │    TEAM         │      │   TEAM      │     │
│  │             │      │                 │      │             │     │
│  │ Event       │      │ Level design,   │      │ Balance,    │     │
│  │ design,     │      │ character art,  │      │ offers,     │     │
│  │ config,     │      │ narrative       │      │ pricing     │     │
│  │ scheduling  │      │                 │      │             │     │
│  └─────────────┘      └─────────────────┘      └─────────────┘     │
│                                                                     │
│  ┌─────────────┐      ┌─────────────────┐      ┌─────────────┐     │
│  │ ENGINEERING │      │   COMMUNITY     │      │  ANALYTICS  │     │
│  │             │      │                 │      │             │     │
│  │ Bug fixes,  │      │ Social, support,│      │ Reporting,  │     │
│  │ stability,  │      │ player comms    │      │ insights,   │     │
│  │ live config │      │                 │      │ A/B tests   │     │
│  └─────────────┘      └─────────────────┘      └─────────────┘     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Current Team Assessment

| Role | Current FTE | Required for Cadence | Gap | Note |
|------|-------------|---------------------|-----|------|
| Live Ops Lead | | | | |
| Event Designer | | | | |
| Content Designer | | | | |
| Economy Designer | | | | |
| Live Engineer | | | | |
| QA (Live) | | | | |
| Community Manager | | | | |
| Analyst | | | | |
| Artist (Live) | | | | |
| Producer (Live) | | | | |

## Framework: Role vs. Workload Mapping

| Function | Hours/Week Required | Who Does It Now | Sustainable? |
|----------|---------------------|-----------------|--------------|
| Event design & config | | | Yes/No |
| Content creation | | | Yes/No |
| Economy tuning | | | Yes/No |
| Bug fixes & stability | | | Yes/No |
| QA for live content | | | Yes/No |
| Community management | | | Yes/No |
| Analytics & reporting | | | Yes/No |
| On-call & incident response | | | Yes/No |
| Feature development | | | Yes/No |

## Framework: Skill Coverage Matrix

| Skill | Person A | Person B | Person C | Person D | Coverage |
|-------|----------|----------|----------|----------|----------|
| Event configuration | ☐ | ☐ | ☐ | ☐ | |
| Economy design | ☐ | ☐ | ☐ | ☐ | |
| Content creation | ☐ | ☐ | ☐ | ☐ | |
| Live engineering | ☐ | ☐ | ☐ | ☐ | |
| Data analysis | ☐ | ☐ | ☐ | ☐ | |
| Community response | ☐ | ☐ | ☐ | ☐ | |
| Incident response | ☐ | ☐ | ☐ | ☐ | |

**Coverage Rating:**
- ✓ = Primary skill
- ~ = Can cover in emergency
- ☐ = Cannot do

**Single Points of Failure:** _______________________

## Framework: Live Ops Team Health Indicators

| Indicator | Healthy | Warning | Critical | Current |
|-----------|---------|---------|----------|---------|
| Event ship rate | >95% on time | 80-95% | <80% | |
| Bug backlog trend | Stable/decreasing | Slowly growing | Rapidly growing | |
| Overtime frequency | Rare | Monthly | Weekly | |
| Sick day usage | Normal | Elevated | High | |
| Role vacancies | None | 1 | >1 | |
| Key person dependencies | None | 1-2 | >2 | |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| Who's overwhelmed? Who's underutilized? | | Rebalancing needed |
| What happens when someone's sick for a week? | | Coverage gaps |
| Are we staffed for average or peak workload? | | Capacity strategy |
| Is anyone doing two full-time jobs? | | Burnout risk |
| When did we last hire for live ops specifically? | | Investment level |

## Framework: Team Evolution Needs

| Current Gap | Options | Recommendation |
|-------------|---------|----------------|
| | Hire / Reassign / Train / Contract / Automate | |
| | | |
| | | |
| | | |

## Checklist

- [ ] Current team roles mapped
- [ ] Workload by function estimated
- [ ] Skill coverage assessed
- [ ] Single points of failure identified
- [ ] Team health indicators tracked
- [ ] Gaps identified with solutions
- [ ] Investment needs documented

## Tasks

1. **Map current team** to live ops functions
2. **Calculate workload** by function per week
3. **Identify coverage gaps** — who can't be sick?
4. **Assess team health indicators**
5. **Create investment case** for needed changes

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.2 Role Clarity Refresh

## Why It Matters

Roles evolve organically as games mature. The person who "just helped with launch" becomes de facto event owner. The engineer who fixed one economy bug becomes the economy engineer. This organic evolution creates confusion—unclear ownership, duplicated effort, and gaps. Regular role clarity refreshes realign reality with intention.

## Framework: Role Evolution Audit

For each team member:

| Person | Original Role | Current Reality | Should Be | Gap |
|--------|---------------|-----------------|-----------|-----|
| | | What they actually do | What we need them to do | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Responsibility Orphans

Responsibilities that have no clear owner:

| Responsibility | Who Does It Now? | Who Should Own It? | Action |
|----------------|------------------|-------------------|--------|
| | Nobody / Whoever notices | | Assign |
| | Multiple people / Unclear | | Clarify |
| | | | |
| | | | |

## Framework: Updated RACI for Live Ops

| Function | Live Ops Lead | Event Designer | Live Engineer | Community | Analyst |
|----------|---------------|----------------|---------------|-----------|---------|
| Event calendar | A | R | C | I | C |
| Event design | C | A/R | C | I | C |
| Event config/deploy | I | C | A/R | I | I |
| Offer design | A | C | I | I | C |
| Balance changes | C | A/R | C | I | R |
| Bug triage | C | C | A/R | C | I |
| Player communication | C | I | I | A/R | I |
| Metrics reporting | C | I | I | I | A/R |
| Incident response | A | I | R | R | R |

## Framework: Role Clarity Conversation

For each team member, discuss:

| Topic | Questions |
|-------|-----------|
| **Core Focus** | What are the 3 most important things you do? |
| **Authority** | What decisions can you make without asking? |
| **Boundaries** | What's explicitly NOT your job? |
| **Dependencies** | Who do you need to do your job? |
| **Conflicts** | Where does your role overlap with others? |
| **Evolution** | How should your role change in 6 months? |

## Framework: Role Documentation Template

### Role: _______________________

**Purpose:** One sentence—why does this role exist?

**Core Responsibilities:**
1.
2.
3.
4.
5.

**Decision Authority:**
- Can decide without approval:
- Must get approval for:

**Key Relationships:**
- Works closely with:
- Receives from:
- Delivers to:

**Success Metrics:**
- 
- 

**Not This Role's Job:**
- 
- 

## Checklist

- [ ] Role evolution audited for each person
- [ ] Orphan responsibilities identified
- [ ] Updated RACI created
- [ ] 1:1 role conversations completed
- [ ] Role documentation updated
- [ ] Team aligned on clarity
- [ ] Review cadence set (quarterly)

## Tasks

1. **Audit each role** — written vs. reality
2. **Identify orphan responsibilities**
3. **Update RACI** for live ops functions
4. **Have role clarity conversations**
5. **Document roles** and share

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.3 Decision-Making Velocity Assessment

## Why It Matters

In live ops, speed matters. A balance decision delayed a week costs revenue. An event approval bottleneck delays the calendar. Slow decisions frustrate teams and slow iteration. Assessing decision-making velocity reveals where you're fast, where you're slow, and why.

## Framework: Decision Velocity Measurement

For recent decisions, track:

| Decision Type | Recent Example | Time to Decide | Ideal Time | Blocker |
|---------------|----------------|----------------|------------|---------|
| Event design approval | | | | |
| Economy balance change | | | | |
| Offer pricing | | | | |
| Bug priority | | | | |
| Feature cut/add | | | | |
| Emergency response | | | | |

**Velocity Rating:**
- Fast: Decided within ideal time
- Slow: 2-3× ideal time
- Blocked: >3× ideal time or stuck

## Framework: Decision Bottleneck Analysis

| Bottleneck Type | Signs | Root Cause | Solution |
|-----------------|-------|------------|----------|
| **Authority unclear** | "Who decides this?" | Missing decision rights | Clarify RACI |
| **Too many approvers** | Long chains | Over-caution culture | Reduce approvers |
| **Information gap** | "Need more data" | Poor data access | Improve dashboards |
| **Meeting dependency** | Waits for weekly meeting | Sync-only decisions | Enable async |
| **Key person unavailable** | One person bottleneck | Over-centralization | Delegate authority |
| **Conflict avoidance** | No one will decide | Fear of being wrong | Safe-to-fail culture |

## Framework: Decision Right Delegation

Decisions that should be delegated:

| Decision | Current Owner | Delegate To | Constraints |
|----------|---------------|-------------|-------------|
| | | | Within budget / parameters |
| | | | |
| | | | |

## Framework: Decision Speed Improvements

| Current State | Target State | Action |
|---------------|--------------|--------|
| All events need Lead approval | Events within template need no approval | Create event templates |
| Balance changes wait for meeting | Balance changes decided within 24h | Daily async review |
| Bug priority escalates | Engineer + QA decide P3-P4 | Delegation |
| Pricing needs exec sign-off | Economy designer decides within ranges | Approved price ranges |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What decision took longest recently? | | Find the bottleneck |
| What's waiting for a decision right now? | | Current blockers |
| Who's the most common bottleneck? | | Delegation opportunity |
| What decisions get made twice? | | Authority confusion |
| What decisions are we avoiding? | | Conflict or fear |

## Checklist

- [ ] Recent decisions tracked with timing
- [ ] Bottlenecks identified
- [ ] Delegation opportunities found
- [ ] Decision speed targets set
- [ ] Changes implemented
- [ ] Velocity re-measured

## Tasks

1. **Track 10 recent decisions** with timing
2. **Identify slowest decision types**
3. **Diagnose bottleneck causes**
4. **Delegate appropriate decisions**
5. **Re-measure in 30 days**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.4 Communication Debt Cleanup

## Why It Matters

Over years, communication patterns accumulate like technical debt. Channels multiply. Meetings add but never subtract. Information lives in unexpected places. New team members can't find anything. Communication debt slows everyone down and creates frustration. Periodic cleanup restores clarity.

## Framework: Communication Audit

### Channel Inventory

| Channel | Purpose | Active Users | Last Active | Keep/Archive/Delete |
|---------|---------|--------------|-------------|---------------------|
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

### Meeting Inventory

| Meeting | Purpose | Attendees | Produces Output? | Keep/Modify/Cut |
|---------|---------|-----------|------------------|-----------------|
| | | | Yes/No | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

### Document Location Audit

| Document Type | Where It Should Be | Where It Actually Is | Fix Needed |
|---------------|-------------------|---------------------|------------|
| Design docs | | | |
| Event configs | | | |
| Runbooks | | | |
| Meeting notes | | | |
| Decisions | | | |

## Framework: Communication Smell Detection

| Smell | Symptom | Fix |
|-------|---------|-----|
| **Channel sprawl** | >20 active channels for small team | Consolidate |
| **Dead channels** | Channels with no posts in 30+ days | Archive |
| **Meeting creep** | >15 hours/week in meetings | Audit and cut |
| **Information scatter** | Same question asked repeatedly | Central docs |
| **Notification fatigue** | People ignore @channel | Reserve for urgent |
| **Email reliance** | Critical info buried in email | Move to channels |
| **Tribal knowledge** | "Ask Sarah, she knows" | Document it |

## Framework: Communication Reset

### Step 1: Audit (Week 1)
- List all channels, meetings, document locations
- Identify what's used, what's not
- Survey team on pain points

### Step 2: Clean (Week 2)
- Archive unused channels
- Cut unnecessary meetings
- Consolidate scattered documents

### Step 3: Clarify (Week 3)
- Document new standards
- Retrain team on expectations
- Update onboarding

### Step 4: Monitor (Ongoing)
- Quarterly mini-audit
- New channel/meeting approval process

## Framework: "Where Does This Go" Quick Reference

Create for your team:

| If you need to... | Use this channel/tool |
|-------------------|----------------------|
| Report a bug | |
| Ask a quick question | |
| Discuss a design | |
| Announce something | |
| Share a document | |
| Escalate an issue | |
| Log a decision | |

## Checklist

- [ ] Channel audit completed
- [ ] Meeting audit completed
- [ ] Document locations mapped
- [ ] Communication smells identified
- [ ] Cleanup executed
- [ ] New standards documented
- [ ] Team retrained
- [ ] Quarterly review scheduled

## Tasks

1. **Inventory all communication channels**
2. **Audit all recurring meetings**
3. **Map document locations**
4. **Identify top 3 communication problems**
5. **Execute cleanup and document standards**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.5 Cross-Team Coordination Optimization

## Why It Matters

Live ops touches everyone—design, engineering, art, QA, marketing, analytics, community. Poor cross-team coordination creates delays, miscommunication, and frustration. As games mature, coordination patterns either improve through learning or degrade through accumulated friction. Regular optimization keeps collaboration healthy.

## Framework: Coordination Touchpoints

| Teams | Coordination Need | Current Mechanism | Friction Level | Improvement |
|-------|-------------------|-------------------|----------------|-------------|
| Design ↔ Engineering | Event implementation | | High/Med/Low | |
| Design ↔ Art | Content assets | | | |
| Engineering ↔ QA | Build handoff | | | |
| LiveOps ↔ Marketing | Event promotion | | | |
| Community ↔ Product | Player feedback | | | |
| Analytics ↔ Design | Data insights | | | |
| LiveOps ↔ Support | Issue awareness | | | |

## Framework: Coordination Mechanisms

| Mechanism | Best For | Cost | Effectiveness |
|-----------|----------|------|---------------|
| Embedded person | Continuous, high-touch | High | High |
| Regular sync meeting | Predictable coordination | Medium | Medium |
| Shared channel | Async, ad-hoc coordination | Low | Medium |
| Liaison role | Occasional, complex coordination | Medium | Medium |
| Shared goals/OKRs | Strategic alignment | Low | High |
| Shared dashboard | Information alignment | Low | Medium |

## Framework: Coordination Friction Sources

| Friction Source | Signs | Solution |
|-----------------|-------|----------|
| **Priority mismatch** | "Not our priority right now" | Shared goals, leadership alignment |
| **Information asymmetry** | "We didn't know about that" | Better communication, dashboards |
| **Process mismatch** | "We work differently" | Align on interfaces, not internals |
| **Resource competition** | "We need them too" | Leadership prioritization |
| **Blame culture** | "It's their fault" | Shared ownership, retrospectives |
| **Physical/time distance** | "They're in a different timezone" | Overlap hours, async-first |

## Framework: Cross-Team Agreement Template

For friction points, create explicit agreements:

### Agreement: [Team A] ↔ [Team B]

**Scope:** What this agreement covers

**Team A commits to:**
- 
- 

**Team B commits to:**
- 
- 

**Communication:**
- Channel:
- Frequency:
- Escalation:

**Review:** [Date] to assess if working

## Framework: Coordination Health Check

| Relationship | Communication | Responsiveness | Quality | Trust | Score |
|--------------|---------------|----------------|---------|-------|-------|
| Design ↔ Engineering | 1-5 | 1-5 | 1-5 | 1-5 | /20 |
| Design ↔ Art | | | | | |
| Engineering ↔ QA | | | | | |
| LiveOps ↔ Marketing | | | | | |
| Community ↔ Product | | | | | |

**Score below 12 = needs intervention**

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| Which cross-team relationship is most painful? | | Focus area |
| Where do handoffs fail most often? | | Process gap |
| Who complains about whom? | | Relationship issue |
| What's the longest cross-team wait time? | | Bottleneck |
| When did teams last align on shared goals? | | Strategic alignment |

## Checklist

- [ ] Coordination touchpoints mapped
- [ ] Friction levels assessed
- [ ] Mechanisms evaluated
- [ ] Agreements created for trouble spots
- [ ] Health check metrics established
- [ ] Regular review scheduled

## Tasks

1. **Map all cross-team touchpoints**
2. **Rate friction level for each**
3. **Diagnose top 3 friction sources**
4. **Create agreements for troubled relationships**
5. **Schedule quarterly coordination health check**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.6 On-Call and Coverage Maturity

## Why It Matters

Live games need live coverage. But immature on-call creates burnout, single points of failure, and delayed response. Mature on-call is sustainable, documented, and resilient. Assessing your on-call maturity reveals where to invest in making it better.

## Framework: On-Call Maturity Model

| Level | Description | Characteristics |
|-------|-------------|-----------------|
| **1 - Ad-hoc** | No formal on-call | One person always responds, no rotation |
| **2 - Basic** | Rotation exists | Schedule exists but gaps, undocumented |
| **3 - Defined** | Formal on-call | Clear rotation, documented procedures, compensation |
| **4 - Robust** | Resilient on-call | Backup coverage, runbooks, low alert noise |
| **5 - Optimized** | Sustainable on-call | Minimal incidents, preventive focus, healthy rotation |

**Current Level:** _______

**Target Level:** _______

## Framework: On-Call Maturity Assessment

| Attribute | Level 1 | Level 3 | Level 5 | Current |
|-----------|---------|---------|---------|---------|
| Schedule | No rotation | Weekly rotation | Rotation with backup | |
| Documentation | None | Basic runbooks | Comprehensive playbooks | |
| Tooling | Phone calls | Paging system | Smart alerting, noise reduction | |
| Compensation | None | Basic | Fair, sustainable | |
| Coverage | One person | Team rotation | Full coverage with backup | |
| Escalation | Undefined | Defined | Practiced, tested | |
| Alert quality | Many false positives | Manageable | Low noise, actionable | |
| Incident learning | Ad-hoc | Post-mortems | Systematic improvement | |

## Framework: Alert Quality Assessment

| Metric | Poor | Good | Excellent | Current |
|--------|------|------|-----------|---------|
| False positive rate | >30% | 10-30% | <10% | |
| Actionable alerts | <50% | 50-80% | >80% | |
| Alert fatigue reports | High | Medium | Low | |
| Duplicate alerts | Common | Occasional | Rare | |
| Response time | >30 min | 15-30 min | <15 min | |

## Framework: On-Call Sustainability Check

| Factor | Sustainable | Concerning | Critical | Current |
|--------|-------------|------------|----------|---------|
| Rotation size | 5+ people | 3-4 people | <3 people | |
| On-call frequency | <1 week/month | 1-2 weeks/month | >2 weeks/month | |
| After-hours incidents | <1/week | 1-3/week | >3/week | |
| Compensation | Fair | Below market | None | |
| Recovery time | Comp time given | Sometimes | Never | |
| Burnout reports | None | Occasional | Frequent | |

## Framework: On-Call Improvement Roadmap

| Level | Actions to Reach |
|-------|------------------|
| 1 → 2 | Create rotation schedule, basic documentation |
| 2 → 3 | Formalize procedures, add compensation, train team |
| 3 → 4 | Add backup coverage, create runbooks, reduce alert noise |
| 4 → 5 | Preventive focus, optimize alerts, continuous improvement |

**Priority improvements:**
1.
2.
3.

## Checklist

- [ ] Maturity level assessed
- [ ] Alert quality measured
- [ ] Sustainability checked
- [ ] Improvement roadmap created
- [ ] Investment needed identified
- [ ] Timeline established

## Tasks

1. **Assess current maturity level** honestly
2. **Measure alert quality** over 2 weeks
3. **Survey team on sustainability**
4. **Create improvement roadmap**
5. **Implement top 3 improvements**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.7 Knowledge Transfer Planning

## Why It Matters

People leave. Without knowledge transfer planning, departure of a key person creates crisis—lost context, broken systems, extended learning curves. Proactive knowledge transfer preserves institutional knowledge and reduces key person risk.

## Framework: Key Person Inventory

| Person | Critical Knowledge | Documentation Level | Backup | Risk |
|--------|-------------------|---------------------|--------|------|
| | | None/Partial/Good | Who else knows | High/Med/Low |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Knowledge Transfer Priority Matrix

```
                     High Criticality
                           │
        ┌──────────────────┼──────────────────┐
        │   URGENT         │   SCHEDULED      │
        │                  │                  │
        │   Transfer NOW   │   Plan transfer  │
        │   Highest risk   │   in next quarter│
        │                  │                  │
   One ─┼──────────────────┼──────────────────┼─ Multiple
 Person │                  │                  │   People
  Knows │   WATCH          │   MAINTAIN       │    Know
        │                  │                  │
        │   Document when  │   Good shape,    │
        │   opportunity    │   light review   │
        │   arises         │                  │
        └──────────────────┼──────────────────┘
                           │
                     Low Criticality
```

## Framework: Knowledge Transfer Methods

| Method | Best For | Time Investment | Effectiveness |
|--------|----------|-----------------|---------------|
| **Pairing** | Complex, tacit knowledge | High | Very High |
| **Documentation** | Explicit, procedural | Medium | Medium |
| **Recording** | Walkthroughs, demos | Medium | Medium |
| **Cross-training** | Role coverage | High | High |
| **Shadow sessions** | Day-in-the-life | Medium | High |
| **Office hours** | Ongoing questions | Low | Medium |

## Framework: Knowledge Transfer Plan Template

### For: [Person/Knowledge Area]

**Knowledge to Transfer:**
1.
2.
3.

**Transfer To:**
- Primary:
- Secondary:

**Method:** Pairing / Documentation / Recording / Training

**Timeline:** _____ weeks

**Success Criteria:** Recipient can [specific capability]

**Progress Tracking:**

| Week | Focus | Deliverable | Status |
|------|-------|-------------|--------|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 | | | |

## Framework: Departure Protocol

When someone gives notice:

### Week 1
- [ ] Identify critical knowledge to transfer
- [ ] Assign recipients
- [ ] Create transfer plan
- [ ] Begin documentation

### Weeks 2-3
- [ ] Execute transfer sessions
- [ ] Create runbooks for their responsibilities
- [ ] Introduce recipients to key contacts
- [ ] Transfer admin access appropriately

### Final Week
- [ ] Complete handoff documentation
- [ ] Validate recipient capability
- [ ] Update RACI
- [ ] Exit interview for knowledge capture
- [ ] Access revocation plan

## Framework: Bus Factor Improvement

| Area | Current Bus Factor | Target | Actions |
|------|-------------------|--------|---------|
| | 1 / 2 / 3+ | 2+ | |
| | | | |
| | | | |
| | | | |

**Bus Factor 1 = High Risk, 2+ = Acceptable**

## Checklist

- [ ] Key people identified
- [ ] Critical knowledge mapped
- [ ] Risk assessed
- [ ] Transfer plans created for high-risk areas
- [ ] Backup people assigned
- [ ] Departure protocol documented
- [ ] Regular review scheduled

## Tasks

1. **Identify key people** and their unique knowledge
2. **Assess documentation level** for each area
3. **Create transfer plans** for high-risk knowledge
4. **Assign backup people** and begin cross-training
5. **Document departure protocol**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.8 Sustainable Pace Enforcement

## Why It Matters

Live ops can be relentless—events never stop, content always needs creating, problems always need fixing. Without intentional sustainable pace, teams slide into chronic overwork. Sustainable pace isn't a luxury; it's the only way to maintain quality and retain talent long-term.

## Framework: Pace Assessment

### Current Workload Analysis

| Team Member | Avg Hours/Week | Overtime Pattern | PTO Last 6 Months | Burnout Risk |
|-------------|----------------|------------------|-------------------|--------------|
| | | Weekly/Monthly/Rare | Days taken | High/Med/Low |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

### Team-Level Indicators

| Indicator | Healthy | Current | Trend |
|-----------|---------|---------|-------|
| Average hours/week | <45 | | ↑↓→ |
| Weekend work frequency | <1/month | | ↑↓→ |
| PTO utilization | >80% | | ↑↓→ |
| Sick day usage | Stable | | ↑↓→ |
| Voluntary turnover | <15%/year | | ↑↓→ |

## Framework: Pace Sustainability Factors

| Factor | Current State | Impact on Pace | Action |
|--------|---------------|----------------|--------|
| Event cadence | | Manageable / Too aggressive | |
| Content velocity | | Sustainable / Straining | |
| Bug backlog | | Under control / Growing | |
| Tool efficiency | | Good / Needs investment | |
| Team size | | Adequate / Understaffed | |
| Planning lead time | | Adequate / Too short | |

## Framework: Sustainable Pace Guidelines

| Guideline | Standard | Your Standard |
|-----------|----------|---------------|
| Standard work week | 40 hours | |
| Maximum sustained | 45 hours | |
| Crunch definition | >50 hours | |
| Crunch limit | 2 weeks max, then mandatory recovery | |
| Weekend work | Emergency only, always comped | |
| PTO encouragement | Active, not just allowed | |
| Focus time | 2+ hours/day uninterrupted | |

## Framework: Pace Protection Mechanisms

| Mechanism | Description | Implemented? |
|-----------|-------------|--------------|
| **Calendar reviews** | Lead reviews team calendars weekly | |
| **Overtime tracking** | Visible tracking of extra hours | |
| **Mandatory comp time** | Overtime triggers automatic recovery | |
| **PTO tracking** | Ensure people take time off | |
| **No-meeting days** | Protected focus time | |
| **On-call limits** | Maximum on-call frequency | |
| **Scope protection** | Push back on unsustainable asks | |
| **Workload discussions** | Regular 1:1 topic | |

## Framework: When Pace Slips

| Symptom | Immediate Action | Longer-term Fix |
|---------|------------------|-----------------|
| Team averaging >45 hours | Audit commitments, cut something | Reduce cadence or add capacity |
| No one taking PTO | Mandate time off | Investigate why people feel they can't |
| Weekend work becoming normal | Stop it, review what's causing | Fix planning or capacity |
| Burnout signals | Individual intervention | Structural fix required |
| Turnover increasing | Exit interviews, rapid assessment | Major intervention |

## Framework: Escalation for Pace Issues

| Situation | Who Escalates | To Whom | Expected Outcome |
|-----------|---------------|---------|------------------|
| Individual overworked | Manager | Lead | Workload redistribution |
| Team overworked | Lead | Director | Scope or capacity change |
| Chronic overtime | Director | Executive | Structural decision |
| Burnout occurring | Anyone | Manager/HR | Immediate intervention |

## Checklist

- [ ] Current pace assessed
- [ ] Unsustainable patterns identified
- [ ] Guidelines established
- [ ] Protection mechanisms implemented
- [ ] Escalation paths clear
- [ ] Regular review scheduled
- [ ] Leadership committed to sustainable pace

## Tasks

1. **Assess current team pace** with data
2. **Identify unsustainable patterns**
3. **Establish pace guidelines** explicitly
4. **Implement protection mechanisms**
5. **Review monthly** and intervene early

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.9 Team Health Intervention

## Why It Matters

Team health problems don't fix themselves—they compound. Dysfunction that's "manageable" becomes culture. Burnout that's "temporary" becomes turnover. Proactive intervention when health indicators decline prevents escalation and preserves the team.

## Framework: Team Health Diagnostic

### Quantitative Indicators

| Indicator | Baseline | Current | Change | Status |
|-----------|----------|---------|--------|--------|
| Pulse survey scores | | | | 🟢🟡🔴 |
| Overtime hours | | | | 🟢🟡🔴 |
| PTO utilization | | | | 🟢🟡🔴 |
| Sick days | | | | 🟢🟡🔴 |
| Turnover (voluntary) | | | | 🟢🟡🔴 |
| Meeting load | | | | 🟢🟡🔴 |

### Qualitative Indicators

| Indicator | Signs | Present? |
|-----------|-------|----------|
| Cynicism | Negative comments, eye-rolling | |
| Withdrawal | Less participation, silence in meetings | |
| Blame | Finger-pointing, defensiveness | |
| Quality decline | More bugs, less care | |
| Communication breakdown | Silos, surprises | |
| Conflict avoidance | Unaddressed tensions | |

## Framework: Health Issue Categorization

| Issue Type | Examples | Intervention Level |
|------------|----------|-------------------|
| **Individual** | One person struggling | Manager 1:1 |
| **Interpersonal** | Conflict between people | Mediation |
| **Team Process** | Bad meetings, unclear roles | Process fix |
| **Team Culture** | Blame, fear, cynicism | Culture intervention |
| **Structural** | Too much work, understaffed | Leadership decision |
| **External** | Company issues, market stress | Communication, support |

## Framework: Intervention Playbook

### For Individual Struggles

1. **Notice** — Watch for signals
2. **Connect** — Private 1:1 conversation
3. **Understand** — Listen without judgment
4. **Support** — Adjust workload, provide resources
5. **Follow up** — Check in regularly

### For Interpersonal Conflict

1. **Assess** — Understand both perspectives
2. **Facilitate** — Mediated conversation
3. **Agree** — Clear agreements forward
4. **Monitor** — Watch for recurrence
5. **Escalate** — If not improving

### For Team-Wide Issues

1. **Diagnose** — Name the problem specifically
2. **Acknowledge** — Don't pretend it's not happening
3. **Engage** — Involve team in solution
4. **Act** — Make concrete changes
5. **Measure** — Track improvement

## Framework: Recovery Planning

When team health is critical:

| Phase | Duration | Focus | Actions |
|-------|----------|-------|---------|
| **Stabilize** | 1-2 weeks | Stop bleeding | Reduce load, address urgent issues |
| **Recover** | 2-4 weeks | Rebuild capacity | Protected time, process fixes |
| **Strengthen** | 4-8 weeks | Prevent recurrence | Structural changes, culture work |
| **Sustain** | Ongoing | Maintain health | Regular monitoring, early intervention |

## Framework: Communication During Intervention

| To Team | Message |
|---------|---------|
| **Acknowledge** | "I know things have been hard. Here's what we're doing about it." |
| **Transparency** | "These are the changes we're making and why." |
| **Invitation** | "I want your input on making this better." |
| **Commitment** | "We're committed to sustainable pace." |

## Framework: Health Intervention Escalation

| Severity | Owner | Actions |
|----------|-------|---------|
| Yellow (concerning) | Manager | 1:1s, minor adjustments |
| Orange (serious) | Manager + Lead | Workload reduction, process changes |
| Red (critical) | Leadership + HR | Major intervention, potential restructure |

## Checklist

- [ ] Health indicators monitored
- [ ] Issues categorized correctly
- [ ] Appropriate intervention selected
- [ ] Recovery plan created if needed
- [ ] Communication planned
- [ ] Escalation path clear
- [ ] Follow-up scheduled

## Tasks

1. **Assess current team health** comprehensively
2. **Categorize issues** by type and severity
3. **Select appropriate interventions**
4. **Communicate with team** about changes
5. **Monitor recovery** and adjust

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3B.10 Stakeholder Relationship Refresh

## Why It Matters

Stakeholder relationships evolve. People change roles. Communication patterns calcify. What worked at launch may not work years later. Regular relationship refresh ensures communication remains effective and expectations stay aligned.

## Framework: Stakeholder Map Update

| Stakeholder | Role | Interest | Influence | Relationship Quality | Last Contact |
|-------------|------|----------|-----------|---------------------|--------------|
| | | | High/Med/Low | Strong/Adequate/Weak | |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |

## Framework: Stakeholder Need Evolution

| Stakeholder | Original Need | Current Need | Change | Adjustment Needed |
|-------------|---------------|--------------|--------|-------------------|
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Communication Effectiveness Assessment

| Stakeholder | Current Mechanism | Frequency | Satisfaction | Improvement |
|-------------|-------------------|-----------|--------------|-------------|
| | | | 1-5 | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Stakeholder Realignment Process

### Step 1: Individual Conversations

**Questions to ask:**
- "What information do you need from us that you're not getting?"
- "What are you getting that you don't need?"
- "How well is our communication working for you?"
- "What decisions do you feel left out of?"
- "What's changed in what you need from our team?"

### Step 2: Communication Plan Update

| Stakeholder | Information Needed | Format | Frequency | Owner |
|-------------|-------------------|--------|-----------|-------|
| | | | | |
| | | | | |
| | | | | |

### Step 3: Alignment Session

If significant misalignment discovered:

| Time | Activity |
|------|----------|
| 10 min | Current state summary |
| 15 min | Stakeholder expectations |
| 15 min | Team capabilities/constraints |
| 15 min | Gap discussion |
| 15 min | Agreement on changes |

## Framework: Stakeholder Satisfaction Survey

Quick quarterly check:

| Question | Scale |
|----------|-------|
| I receive the information I need | 1-5 |
| Communication frequency is right | 1-5 |
| I'm included in appropriate decisions | 1-5 |
| The team is responsive to my needs | 1-5 |
| Overall satisfaction with relationship | 1-5 |

## Checklist

- [ ] Stakeholder map updated
- [ ] Needs evolution assessed
- [ ] Communication effectiveness reviewed
- [ ] Individual conversations held
- [ ] Communication plan updated
- [ ] Alignment session held if needed
- [ ] Satisfaction survey scheduled

## Tasks

1. **Update stakeholder map** with current roles
2. **Assess relationship quality** honestly
3. **Conduct individual conversations**
4. **Update communication plan**
5. **Schedule regular satisfaction checks**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# Track B Summary

## Live Ops Team Structure Checklist

Before proceeding to Block 4B (Operational Excellence), confirm:

| Team Structure Element | Complete? | Key Finding |
|-----------------------|-----------|-------------|
| Team Structure Assessment | | |
| Role Clarity Refresh | | |
| Decision Velocity Assessment | | |
| Communication Debt Cleanup | | |
| Cross-Team Coordination | | |
| On-Call Maturity | | |
| Knowledge Transfer Planning | | |
| Sustainable Pace Enforcement | | |
| Team Health Intervention | | |
| Stakeholder Relationship Refresh | | |

## Key Outputs from Block 3B

| Output | Location | Owner |
|--------|----------|-------|
| Updated team structure | | |
| Refreshed RACI | | |
| Communication standards | | |
| On-call improvement plan | | |
| Knowledge transfer plans | | |
| Team health dashboard | | |
| Stakeholder communication plan | | |

## Red Flags Requiring Attention

- [ ] Key person dependencies unaddressed
- [ ] Decision velocity slow for live ops needs
- [ ] Communication channels cluttered
- [ ] On-call not sustainable
- [ ] Team health declining
- [ ] Stakeholder relationships strained
- [ ] No knowledge transfer happening

---

# Block 3 Complete

## Next Steps

**From Track A:** Proceed to Block 4A (Daily Production & Execution) for production processes.

**From Track B:** Proceed to Block 4B (Operational Excellence) for live ops execution optimization.

---

*"The strength of the team is each individual member. The strength of each member is the team."*  
— Phil Jackson

---
