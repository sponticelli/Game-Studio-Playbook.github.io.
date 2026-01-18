---
layout: default
title: "Team Structure and Communication"
---

# Team Structure & Communication

> *"Culture eats strategy for breakfast, but structure eats culture for lunch."*  
> — Adapted from Peter Drucker

---

# TRACK A: Team Structure & Communication (Greenfield Projects)

Complete these topics before entering full production. Return to them when communication breaks down or roles become unclear.

---

# 3A.1 Role & Responsibility Matrix (RACI)

## Why It Matters

"Everyone owns it" means no one owns it. When responsibilities are unclear, work falls through cracks, gets duplicated, or stalls waiting for someone to claim it. A RACI matrix makes accountability explicit, prevents conflicts, and speeds decision-making by eliminating "who should handle this?" conversations.

## Framework: RACI Definitions

| Letter | Role | Definition | Rules |
|--------|------|------------|-------|
| **R** | Responsible | Does the work | At least one per task, can be multiple |
| **A** | Accountable | Makes final decision, owns outcome | Exactly ONE per task, never shared |
| **C** | Consulted | Provides input before decision | Two-way communication |
| **I** | Informed | Told after decision | One-way communication |

```
                    ┌─────────────────────────────────────────┐
                    │           RACI RELATIONSHIP             │
                    └─────────────────────────────────────────┘
                                       │
           ┌───────────────────────────┼───────────────────────────┐
           │                           │                           │
           ▼                           ▼                           ▼
    ┌─────────────┐             ┌─────────────┐             ┌─────────────┐
    │ ACCOUNTABLE │◄───────────▶│ RESPONSIBLE │◄───────────▶│  CONSULTED  │
    │             │   Approves   │             │   Asks for  │             │
    │  One person │    work      │  Does work  │    input    │ Gives input │
    │  owns it    │             │             │             │             │
    └─────────────┘             └──────┬──────┘             └─────────────┘
                                       │
                                       │ Notifies
                                       ▼
                                ┌─────────────┐
                                │  INFORMED   │
                                │             │
                                │ Receives    │
                                │ updates     │
                                └─────────────┘
```

## Framework: Core RACI Matrix

### Game Development Functions

| Function/Decision | Producer | Game Designer | Lead Engineer | Art Director | QA Lead | Marketing |
|-------------------|----------|---------------|---------------|--------------|---------|-----------|
| **Vision & Pillars** | A | R | C | C | I | C |
| **Feature Scope** | A | R | C | C | I | I |
| **Feature Design** | C | A/R | C | C | I | I |
| **Technical Architecture** | C | C | A/R | I | I | I |
| **Art Direction** | C | C | I | A/R | I | C |
| **Audio Direction** | C | C | I | C | I | I |
| **Sprint Planning** | A | R | R | R | C | I |
| **Bug Prioritization** | C | C | C | I | A/R | I |
| **Release Decisions** | A | C | C | C | C | C |
| **Milestone Sign-off** | A | R | R | R | R | I |
| **Marketing Messaging** | C | C | I | C | I | A/R |
| **Pricing Decisions** | A | C | I | I | I | C |
| **Live Ops Calendar** | A | R | C | C | I | C |
| **Economy Design** | C | A/R | C | I | C | I |
| **Monetization Design** | A | R | C | I | I | C |
| **Community Response** | C | C | I | I | I | A/R |
| **Hiring Decisions** | A | C | C | C | I | I |

### Your Project RACI

| Function/Decision | _______ | _______ | _______ | _______ | _______ | _______ |
|-------------------|---------|---------|---------|---------|---------|---------|
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |

## Framework: RACI Validation Rules

| Rule | Check | Pass? |
|------|-------|-------|
| Every row has exactly one "A" | Count A's per row | |
| Every row has at least one "R" | Count R's per row | |
| No row is all "I"s | At least one R, A, or C | |
| No person is "A" for everything | Distributed accountability | |
| "A" has authority to make decision | Real power matches | |
| "C" people are actually consulted | Not just informed | |
| Nobody is overloaded | Reasonable R count | |

## Framework: Common RACI Anti-Patterns

| Anti-Pattern | Symptom | Fix |
|--------------|---------|-----|
| **Consensus Creep** | Multiple A's | One person must own it |
| **Hero Syndrome** | One person is A/R for everything | Distribute accountability |
| **RACI Theater** | Matrix exists but ignored | Enforce in practice |
| **Consultation Overload** | Everyone is C | Limit to true stakeholders |
| **Accountability Avoidance** | No one wants A | Leadership must assign |
| **Missing Informed** | Surprises and conflicts | Add appropriate I's |

## Framework: Role Definition Template

For each key role, define clearly:

### Role: _______________________

| Attribute | Definition |
|-----------|------------|
| **Core Responsibilities** | What do they own? |
| **Key Decisions** | What can they decide without escalation? |
| **Deliverables** | What do they produce? |
| **Interfaces** | Who do they work with most? |
| **Reports To** | Who is their accountable party? |
| **Success Metrics** | How is their performance measured? |

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

## Checklist

- [ ] RACI matrix created for all major functions
- [ ] Every row has exactly one "A"
- [ ] No single person owns too many "A"s
- [ ] All team members reviewed and understand their assignments
- [ ] "A" parties have actual authority to make decisions
- [ ] Matrix is posted/accessible to all team members
- [ ] Review cadence established (quarterly recommended)

## Tasks

1. **List all key decisions/functions** for your project
2. **Assign RACI** for each with your team present
3. **Validate against rules** — check for anti-patterns
4. **Get explicit agreement** from each "A" party
5. **Post visibly** and reference in decision discussions

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.2 Decision Rights by Domain

## Why It Matters

RACI shows who's responsible, but decision rights define the *boundaries* of authority. Without clear decision rights, small decisions escalate unnecessarily, slowing velocity, or big decisions get made by people without full context. Defined decision rights empower the team while protecting strategic alignment.

## Framework: Decision Rights Tiers

```
┌─────────────────────────────────────────────────────────────────────┐
│                    DECISION RIGHTS PYRAMID                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                         ┌───────────┐                               │
│                         │  TIER 1   │                               │
│                         │ Strategic │ Vision, kill, major pivot     │
│                         │  ◀ EXEC ▶ │                               │
│                         └─────┬─────┘                               │
│                               │                                     │
│                    ┌──────────┴──────────┐                          │
│                    │       TIER 2        │                          │
│                    │     Significant     │ Scope, timeline, major   │
│                    │   ◀ LEADERSHIP ▶    │ feature decisions        │
│                    └──────────┬──────────┘                          │
│                               │                                     │
│               ┌───────────────┴───────────────┐                     │
│               │           TIER 3              │                     │
│               │         Tactical              │ Sprint scope, task  │
│               │      ◀ TEAM LEADS ▶           │ priorities, solutions│
│               └───────────────┬───────────────┘                     │
│                               │                                     │
│         ┌─────────────────────┴─────────────────────┐               │
│         │                 TIER 4                    │               │
│         │              Operational                  │ Implementation │
│         │           ◀ INDIVIDUAL ▶                  │ details, methods│
│         └───────────────────────────────────────────┘               │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Domain-Specific Decision Rights

### Game Design Domain

| Decision Type | Who Decides | Consulted | Escalation Trigger |
|---------------|-------------|-----------|-------------------|
| Core mechanic changes | Game Director | Engineering, Producer | Player-facing impact |
| Level/content balance | Lead Designer | QA, Analytics | Economy impact |
| Difficulty tuning | Designer | QA | Affects progression |
| UI/UX flow | UX Designer | Engineering | Major rework needed |
| Economy values | Economy Designer | Producer, Analytics | Revenue impact |
| Event design | Live Ops Designer | Engineering, QA | Technical constraints |

### Engineering Domain

| Decision Type | Who Decides | Consulted | Escalation Trigger |
|---------------|-------------|-----------|-------------------|
| Architecture decisions | Tech Lead | Engineering team | Long-term implications |
| Technology/library selection | Tech Lead | Team | Cost or licensing |
| Code standards | Tech Lead | Team | Team objection |
| Bug fix approach | Assigned engineer | QA, Lead | Risky changes |
| Performance optimization | Engineer | Lead | Affects features |
| Technical debt paydown | Tech Lead | Producer | Schedule impact |

### Art Domain

| Decision Type | Who Decides | Consulted | Escalation Trigger |
|---------------|-------------|-----------|-------------------|
| Visual style/direction | Art Director | Design, Marketing | Brand impact |
| Asset specifications | Art Lead | Engineering | Technical constraints |
| Animation approach | Animation Lead | Design | Gameplay impact |
| Outsourcing decisions | Art Director | Producer | Budget impact |
| Quality vs. schedule | Art Director | Producer | Deadline risk |

### Production Domain

| Decision Type | Who Decides | Consulted | Escalation Trigger |
|---------------|-------------|-----------|-------------------|
| Sprint content | Producer | Leads | Capacity exceeded |
| Schedule adjustments | Producer | Leads, Stakeholders | Milestone impact |
| Resource allocation | Producer | Leads | Cross-team impact |
| Risk responses | Producer | Leads | Budget/timeline impact |
| Process changes | Producer | Team | Team resistance |
| External communication | Producer | Marketing, Leads | Public-facing |

### Your Decision Rights Matrix

| Domain | Decision Type | Decides | Consults | Escalates When |
|--------|---------------|---------|----------|----------------|
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Escalation Criteria

| Criteria | Examples | Escalate To |
|----------|----------|-------------|
| **Budget Impact** | >$X or >Y% of budget | Producer → Exec |
| **Timeline Impact** | >1 week slip | Producer |
| **Scope Impact** | Feature cut or major addition | Producer → Stakeholders |
| **Quality Impact** | Ship with known issue | Producer → Stakeholders |
| **Team Impact** | Affects multiple teams | Producer |
| **Player Impact** | Changes promised features | Leadership |
| **Revenue Impact** | Affects monetization | Leadership → Exec |
| **Legal/Compliance** | Any legal concerns | Legal → Exec |

## Framework: Decision Speed by Type

| Decision Type | Target Time | Who | Documentation |
|---------------|-------------|-----|---------------|
| Operational (Tier 4) | Same day | Individual | None required |
| Tactical (Tier 3) | 1-2 days | Lead | Team notes |
| Significant (Tier 2) | 1 week | Leadership | Decision log |
| Strategic (Tier 1) | 2-4 weeks | Executive | Formal document |

## Framework: Decision Log Template

For Tier 1-2 decisions, document:

| Field | Content |
|-------|---------|
| **Decision ID** | |
| **Date** | |
| **Decision** | |
| **Decider** | |
| **Context** | Why was this needed? |
| **Options Considered** | |
| **Rationale** | Why this choice? |
| **Consulted** | Who provided input? |
| **Impact** | What does this affect? |
| **Reversibility** | Can we change course? |

## Checklist

- [ ] Decision tiers defined
- [ ] Domain-specific rights documented
- [ ] Escalation criteria clear
- [ ] Decision speed expectations set
- [ ] Decision log template created
- [ ] Team understands their authority
- [ ] Escalation paths known

## Tasks

1. **Map decisions by domain** for your project
2. **Assign decision rights** for each type
3. **Define escalation triggers** clearly
4. **Set response time expectations**
5. **Create and maintain decision log** for major decisions

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.3 Handoff Protocol Design

## Why It Matters

Work crosses boundaries constantly: Design → Engineering → Art → QA → Release. Each handoff is a potential failure point where context is lost, requirements are misunderstood, or work sits waiting. Structured handoff protocols ensure smooth transitions and reduce "throw it over the wall" dysfunction.

## Framework: Handoff Map

```
┌─────────────────────────────────────────────────────────────────────┐
│                      PRODUCTION HANDOFF FLOW                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌──────────┐      ┌──────────┐      ┌──────────┐      ┌──────────┐│
│  │  DESIGN  │─────▶│ENGINEERING─────▶│   ART    │─────▶│INTEGRATION│
│  │          │  H1  │          │  H2  │          │  H3  │          ││
│  └──────────┘      └──────────┘      └──────────┘      └──────────┘│
│                                                               │     │
│                                                               │ H4  │
│                                                               ▼     │
│  ┌──────────┐      ┌──────────┐      ┌──────────┐      ┌──────────┐│
│  │  LIVE    │◀─────│ RELEASE  │◀─────│ STAGING  │◀─────│    QA    ││
│  │          │  H7  │          │  H6  │          │  H5  │          ││
│  └──────────┘      └──────────┘      └──────────┘      └──────────┘│
│                                                                     │
│  H = Handoff Point                                                  │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Handoff Protocol Template

### Handoff: Design → Engineering

| Element | Requirement |
|---------|-------------|
| **Trigger** | Design spec marked "Ready for Engineering" |
| **Artifacts Required** | |
| | - Feature specification document |
| | - Wireframes/mockups |
| | - User flow diagrams |
| | - Edge case documentation |
| | - Acceptance criteria |
| **Quality Gate** | Design review completed with engineering present |
| **Handoff Meeting** | 30-minute kickoff with Q&A |
| **Recipient Confirms** | Engineering acknowledges receipt and timeline |
| **Escalation** | If blocked >24 hours, escalate to Producer |

### Handoff: Engineering → QA

| Element | Requirement |
|---------|-------------|
| **Trigger** | Feature marked "Ready for QA" in tracking |
| **Artifacts Required** | |
| | - Working build |
| | - Test instructions |
| | - Known limitations |
| | - Related bug fixes included |
| **Quality Gate** | Developer self-test completed |
| **Handoff Meeting** | Async with Slack/message summary |
| **Recipient Confirms** | QA acknowledges and provides timeline |
| **Escalation** | If build broken, immediate return to Engineering |

### Handoff: QA → Release

| Element | Requirement |
|---------|-------------|
| **Trigger** | QA sign-off in tracking system |
| **Artifacts Required** | |
| | - Test report |
| | - Known shippable issues list |
| | - Regression results |
| | - Performance metrics |
| **Quality Gate** | All critical/blocker bugs resolved |
| **Handoff Meeting** | Release readiness meeting |
| **Recipient Confirms** | Release manager approves |
| **Escalation** | Any critical issues → Leadership decision |

### Handoff: Release → Live Ops

| Element | Requirement |
|---------|-------------|
| **Trigger** | Successful deployment |
| **Artifacts Required** | |
| | - Release notes |
| | - Config changes documented |
| | - Rollback plan |
| | - Known issues for support |
| **Quality Gate** | Smoke test in production passed |
| **Handoff Meeting** | Brief handoff call or async update |
| **Recipient Confirms** | Live Ops acknowledges and begins monitoring |
| **Escalation** | Any production issues → Incident response |

## Framework: Handoff Checklist Template

### Pre-Handoff (Sender)

- [ ] All required artifacts complete
- [ ] Self-review/test completed
- [ ] Quality gate passed
- [ ] Recipient notified
- [ ] Handoff meeting scheduled (if required)
- [ ] Documentation accessible

### Handoff Moment

- [ ] Walk through work completed
- [ ] Answer recipient questions
- [ ] Confirm understanding
- [ ] Agree on timeline
- [ ] Document any open items

### Post-Handoff (Recipient)

- [ ] Acknowledge receipt
- [ ] Validate artifacts received
- [ ] Identify any gaps immediately
- [ ] Begin work or schedule start
- [ ] Update tracking system

## Framework: Your Project Handoffs

| Handoff | From | To | Trigger | Key Artifacts | Meeting? |
|---------|------|-----|---------|---------------|----------|
| H1 | | | | | |
| H2 | | | | | |
| H3 | | | | | |
| H4 | | | | | |
| H5 | | | | | |
| H6 | | | | | |
| H7 | | | | | |

## Framework: Handoff Anti-Patterns

| Anti-Pattern | Symptom | Fix |
|--------------|---------|-----|
| **Throw Over the Wall** | No context transferred | Require handoff meeting |
| **Incomplete Artifacts** | Frequent questions after handoff | Quality gate before handoff |
| **No Acknowledgment** | Work sits in limbo | Require explicit receipt |
| **Verbal Only** | "I told them" disputes | Document in tracking system |
| **Premature Handoff** | Work returned frequently | Stronger quality gates |
| **Handoff Bottleneck** | One person reviews everything | Distribute handoff rights |

## Checklist

- [ ] All handoff points identified
- [ ] Protocol defined for each handoff
- [ ] Required artifacts listed
- [ ] Quality gates established
- [ ] Escalation paths clear
- [ ] Team trained on protocols
- [ ] Tracking system supports handoff status

## Tasks

1. **Map your handoff points** in the production flow
2. **Define protocol** for each handoff
3. **Create artifact checklists** for each
4. **Establish quality gates**
5. **Train team** on handoff expectations

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.4 Meeting Taxonomy

## Why It Matters

Meetings are expensive—a 1-hour meeting with 8 people costs 8 person-hours. Yet many teams drown in meetings that lack purpose, wrong attendees, or no outcomes. A meeting taxonomy defines which meetings exist, why they exist, and how to run them effectively. Bad meetings destroy productivity; good meetings accelerate it.

## Framework: Meeting Categories

```
┌─────────────────────────────────────────────────────────────────────┐
│                       MEETING CATEGORIES                            │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐     │
│  │   ALIGNMENT     │  │    WORKING      │  │    DECISION     │     │
│  │                 │  │                 │  │                 │     │
│  │ Share info,     │  │ Create output   │  │ Make choices    │     │
│  │ coordinate      │  │ together        │  │                 │     │
│  │                 │  │                 │  │                 │     │
│  │ Stand-ups,      │  │ Design reviews, │  │ Prioritization, │     │
│  │ All-hands,      │  │ Brainstorms,    │  │ Go/No-Go,       │     │
│  │ Status updates  │  │ Workshops       │  │ Triage          │     │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘     │
│                                                                     │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐     │
│  │   FEEDBACK      │  │    SOCIAL       │  │    CRISIS       │     │
│  │                 │  │                 │  │                 │     │
│  │ Improve process │  │ Build team      │  │ Respond to      │     │
│  │ or work         │  │ cohesion        │  │ incidents       │     │
│  │                 │  │                 │  │                 │     │
│  │ Retrospectives, │  │ Team building,  │  │ War rooms,      │     │
│  │ 1:1s, Reviews   │  │ Celebrations    │  │ Incident calls  │     │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Meeting Catalog

### Alignment Meetings

| Meeting | Purpose | Frequency | Duration | Attendees | Output |
|---------|---------|-----------|----------|-----------|--------|
| **Daily Stand-up** | Sync on progress, blockers | Daily | 15 min | Core team | Blockers identified |
| **Weekly Status** | Review progress against plan | Weekly | 30-60 min | Team + Stakeholders | Status report |
| **Sprint Review** | Demo completed work | Per sprint | 1 hour | Team + Stakeholders | Feedback captured |
| **All-Hands** | Broad team alignment | Monthly | 30-60 min | Everyone | Shared context |

### Working Meetings

| Meeting | Purpose | Frequency | Duration | Attendees | Output |
|---------|---------|-----------|----------|-----------|--------|
| **Design Review** | Critique and improve designs | As needed | 1 hour | Design + relevant | Approved design |
| **Sprint Planning** | Plan next sprint work | Per sprint | 2 hours | Team | Sprint backlog |
| **Brainstorm** | Generate ideas | As needed | 1-2 hours | Cross-functional | Idea list |
| **Workshop** | Solve specific problem | As needed | 2-4 hours | Relevant experts | Solution or plan |

### Decision Meetings

| Meeting | Purpose | Frequency | Duration | Attendees | Output |
|---------|---------|-----------|----------|-----------|--------|
| **Prioritization** | Rank work items | Per sprint | 1 hour | Leads + Producer | Prioritized backlog |
| **Triage** | Assess issues | As needed | 30 min | QA + Leads | Triaged bug list |
| **Go/No-Go** | Milestone decision | Per milestone | 1-2 hours | Stakeholders | Decision documented |
| **Feature Cut** | Scope reduction | As needed | 1 hour | Leads + Producer | Cut list |

### Feedback Meetings

| Meeting | Purpose | Frequency | Duration | Attendees | Output |
|---------|---------|-----------|----------|-----------|--------|
| **Retrospective** | Process improvement | Per sprint | 1 hour | Team | Action items |
| **1:1** | Individual sync | Weekly | 30 min | Manager + Report | Notes, actions |
| **Playtest Debrief** | Analyze playtest results | After playtests | 1 hour | Team | Findings list |
| **Post-Mortem** | Learn from incidents | After incidents | 1-2 hours | Involved parties | Improvements |

## Framework: Meeting Template

### Meeting: _______________________

| Field | Specification |
|-------|---------------|
| **Purpose** | Why does this meeting exist? |
| **Frequency** | How often? |
| **Duration** | How long? (max) |
| **Required Attendees** | Who must be there? |
| **Optional Attendees** | Who might benefit? |
| **Facilitator** | Who runs it? |
| **Agenda Template** | Standard structure |
| **Pre-Work** | What should people do before? |
| **Output** | What should exist after? |
| **Cancellation Criteria** | When to skip? |

## Framework: Daily Stand-up Protocol

| Element | Specification |
|---------|---------------|
| **Time** | Same time daily, preferably morning |
| **Duration** | 15 minutes MAXIMUM |
| **Format** | Standing (in-person) or cameras on |
| **Structure** | Round-robin or walk-the-board |

**Each Person Answers:**
1. What did I complete since last standup?
2. What will I work on today?
3. What's blocking me?

**Rules:**
- No problem-solving in standup
- Deep discussions → "parking lot" for after
- Start on time, end on time
- Missing? Send async update

## Framework: Effective Meeting Principles

| Principle | Implementation |
|-----------|----------------|
| **Has a Purpose** | State purpose in invite |
| **Right People** | Only those needed, no more |
| **Has an Agenda** | Sent in advance |
| **Starts on Time** | Don't wait for latecomers |
| **Has a Facilitator** | Someone runs it |
| **Ends with Actions** | Who does what by when |
| **Respects Time** | End on time or early |
| **Has Notes** | Document outcomes |

## Framework: Meeting Audit

| Meeting | Purpose Clear? | Right Attendees? | Produces Output? | Keep/Modify/Cut |
|---------|----------------|------------------|------------------|-----------------|
| | Yes/No | Yes/No | Yes/No | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Your Meeting Calendar

| Day | Morning | Midday | Afternoon |
|-----|---------|--------|-----------|
| Monday | | | |
| Tuesday | | | |
| Wednesday | | | |
| Thursday | | | |
| Friday | | | |

**Protected Focus Time:** _______________________

**No-Meeting Day:** _______________________

## Checklist

- [ ] All necessary meetings identified
- [ ] Purpose defined for each meeting
- [ ] Duration limits set
- [ ] Attendee lists appropriate
- [ ] Facilitators assigned
- [ ] Agenda templates created
- [ ] Team calendar reflects meetings
- [ ] Focus time protected
- [ ] Meeting audit scheduled (quarterly)

## Tasks

1. **Inventory current meetings** — list all recurring meetings
2. **Audit each meeting** — does it need to exist?
3. **Define protocols** for remaining meetings
4. **Create agenda templates** for each
5. **Block focus time** and protect it

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.5 Live Ops War Room Protocol

## Why It Matters

Events and launches go wrong. Servers crash. Exploits are discovered. When things break, you need instant coordination—not "who should I call?" panic. A war room protocol defines how to assemble, communicate, and resolve crises. Practiced in advance, it becomes automatic when needed.

## Framework: War Room Activation Criteria

| Severity | Trigger | War Room? | Response |
|----------|---------|-----------|----------|
| **Critical** | Game unplayable, data loss, major exploit | Yes, immediate | Full war room |
| **High** | Significant issue, partial outage | Yes, within 1 hour | Core team |
| **Medium** | Noticeable issue, workarounds exist | No | On-call + relevant |
| **Low** | Minor issue | No | Normal process |

## Framework: War Room Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                      WAR ROOM STRUCTURE                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                      ┌───────────────────┐                          │
│                      │    INCIDENT       │                          │
│                      │    COMMANDER      │                          │
│                      │  (Owns response)  │                          │
│                      └─────────┬─────────┘                          │
│                                │                                    │
│         ┌──────────────────────┼──────────────────────┐             │
│         │                      │                      │             │
│         ▼                      ▼                      ▼             │
│  ┌─────────────┐      ┌─────────────┐      ┌─────────────┐         │
│  │  TECHNICAL  │      │   COMMS     │      │    DATA     │         │
│  │    LEAD     │      │    LEAD     │      │    LEAD     │         │
│  │             │      │             │      │             │         │
│  │ Diagnosis & │      │ Player &    │      │ Impact      │         │
│  │ fix         │      │ stakeholder │      │ assessment  │         │
│  └─────────────┘      └─────────────┘      └─────────────┘         │
│         │                      │                      │             │
│         ▼                      ▼                      ▼             │
│  ┌─────────────┐      ┌─────────────┐      ┌─────────────┐         │
│  │  Engineers  │      │  Community  │      │  Analytics  │         │
│  │     QA      │      │   Support   │      │             │         │
│  └─────────────┘      └─────────────┘      └─────────────┘         │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: War Room Roles

| Role | Responsibility | Required Skills | Primary | Backup |
|------|----------------|-----------------|---------|--------|
| **Incident Commander** | Overall coordination, decisions, timeline | Leadership, calm under pressure | | |
| **Technical Lead** | Diagnosis, fix implementation | System expertise | | |
| **Comms Lead** | Player communication, stakeholder updates | Communication, empathy | | |
| **Data Lead** | Impact assessment, monitoring | Analytics, queries | | |

## Framework: War Room Activation Checklist

### Immediately (0-5 minutes)

- [ ] Incident detected/reported
- [ ] Initial severity assessment
- [ ] War room activation decision
- [ ] Incident Commander assigned
- [ ] War room channel/call created
- [ ] Core team paged/notified

### Setup (5-15 minutes)

- [ ] All required roles present
- [ ] Incident brief shared
- [ ] Initial impact assessment
- [ ] First player communication drafted
- [ ] Stakeholders notified
- [ ] Update cadence established

### Active Response

- [ ] Regular status updates (every 15-30 min)
- [ ] Player communication maintained
- [ ] Fix in progress
- [ ] Impact monitored
- [ ] Decision log maintained
- [ ] Stakeholder updates continued

### Resolution

- [ ] Fix deployed and verified
- [ ] Player communication sent
- [ ] Monitoring confirmed stable
- [ ] War room closed
- [ ] Post-mortem scheduled
- [ ] Compensation determined (if applicable)

## Framework: Communication Templates

### Internal Status Update (Every 15-30 min)

```
[TIME] WAR ROOM UPDATE - [INCIDENT]
Status: Active/Mitigated/Resolved
Impact: [Brief description]
Current action: [What we're doing]
Next update: [Time]
Blockers: [If any]
```

### Player Communication - Acknowledgment

```
We're aware of [issue] and our team is actively working on it. 
We'll share updates as we learn more. Thank you for your patience.
```

### Player Communication - Update

```
Update on [issue]: [Current status]
Our team is [action]. We expect [timeline if known].
We'll continue to keep you updated.
```

### Player Communication - Resolution

```
[Issue] has been resolved. 
[Brief explanation]
[Compensation if applicable]
Thank you for your patience. We're taking steps to prevent this in the future.
```

## Framework: Decision Log Template

| Time | Decision | Made By | Rationale | Outcome |
|------|----------|---------|-----------|---------|
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: War Room Tools

| Tool | Purpose | Your Tool |
|------|---------|-----------|
| Communication channel | Real-time coordination | |
| Video call | Face-to-face if needed | |
| Incident tracking | Log events, actions | |
| Monitoring dashboard | Watch recovery | |
| Runbook repository | Access playbooks | |
| Player communication | Push updates | |

## Checklist

- [ ] War room activation criteria defined
- [ ] Roles assigned with backups
- [ ] Communication channel ready
- [ ] Communication templates prepared
- [ ] Paging/alerting configured
- [ ] Tools identified and tested
- [ ] Runbooks accessible
- [ ] Team trained on protocol

## Tasks

1. **Define activation criteria** for your game
2. **Assign roles** with backup coverage
3. **Create communication channel** (always available)
4. **Prepare templates** for common scenarios
5. **Run a drill** — practice with fake incident

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.6 Stand-up / Check-in Format

## Why It Matters

Stand-ups are the heartbeat of team coordination. Done well, they surface blockers early, build accountability, and keep everyone aligned. Done poorly, they become status theater that wastes time. The format matters: it should be quick, focused, and actionable.

## Framework: Stand-up Formats

| Format | Best For | Duration | Structure |
|--------|----------|----------|-----------|
| **Round-Robin** | Small teams (<8) | 10-15 min | Each person reports |
| **Walk-the-Board** | Kanban teams | 10-20 min | Review each card |
| **Exception-Based** | Mature teams | 5-10 min | Only blockers/changes |
| **Async Stand-up** | Remote/distributed | N/A | Written updates |

## Framework: Round-Robin Format

```
┌─────────────────────────────────────────────────────────────────────┐
│                    ROUND-ROBIN STAND-UP                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  Each person answers THREE questions (30-60 seconds max):           │
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  1. What did I COMPLETE since last stand-up?                │    │
│  │     (Not "worked on" — completed)                           │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  2. What will I COMPLETE by next stand-up?                  │    │
│  │     (Commitment, not hope)                                  │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  3. What's BLOCKING me?                                     │    │
│  │     (Not "might block" — is blocking)                       │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Walk-the-Board Format

```
┌─────────────────────────────────────────────────────────────────────┐
│                    WALK-THE-BOARD STAND-UP                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  Review board RIGHT to LEFT (done → doing → to do):                 │
│                                                                     │
│  TO DO          IN PROGRESS       IN REVIEW         DONE           │
│  ┌─────┐        ┌─────┐           ┌─────┐          ┌─────┐         │
│  │     │        │ 3   │◀──────────│ 2   │◀─────────│ 1   │         │
│  │     │        │     │    ◀──────│     │    ◀─────│     │         │
│  │ 6   │        │ 4   │           │     │          │     │         │
│  │     │        │     │           │     │          │     │         │
│  │     │        │ 5   │           │     │          │     │         │
│  └─────┘        └─────┘           └─────┘          └─────┘         │
│                                                                     │
│  For each card:                                                     │
│  - Any blockers?                                                    │
│  - Need anything?                                                   │
│  - On track for commitment?                                         │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Async Stand-up Format

**For distributed or timezone-spread teams:**

### Daily Update Template (Slack/Channel)

```
📅 [Date] Stand-up - [Name]

✅ Completed:
- [Item 1]
- [Item 2]

🎯 Today:
- [Item 1]
- [Item 2]

🚧 Blockers:
- [None / Description]

📝 Notes:
- [Optional context]
```

### Async Stand-up Rules

| Rule | Rationale |
|------|-----------|
| Post by [time] daily | Consistency |
| Use thread for questions | Keep channel clean |
| Blockers get immediate response | Don't wait for standup |
| Missed update = 1:1 check-in | Ensure people aren't stuck |

## Framework: Stand-up Anti-Patterns

| Anti-Pattern | Symptom | Fix |
|--------------|---------|-----|
| **Status Reports** | Listing activities not outcomes | Focus on "completed" and "blocked" |
| **Problem Solving** | Discussion takes over | "Parking lot" for after |
| **Late Starts** | Waiting for stragglers | Start on time, every time |
| **Long Duration** | Exceeds 15 minutes | Enforce time, cut discussion |
| **Audience Mode** | Only PM pays attention | Everyone stands, cameras on |
| **No Blockers** | No one ever blocked | Challenge — there are always blockers |
| **Blame Game** | Pointing fingers | Focus on work, not people |

## Framework: Parking Lot Protocol

When topics need discussion:

1. **Capture it:** "That's a parking lot item"
2. **Note who's needed:** "Sarah and Mike, let's talk after"
3. **Continue stand-up:** Don't derail
4. **Address immediately after:** Solve while context is fresh

### Parking Lot Template

| Topic | Raised By | Needed | Resolved |
|-------|-----------|--------|----------|
| | | | ☐ |
| | | | ☐ |
| | | | ☐ |

## Framework: Stand-up Facilitation

| Facilitator Action | When | How |
|--------------------|------|-----|
| Start on time | Always | "Let's begin" — don't wait |
| Keep moving | Someone goes long | "Let's take that offline" |
| Note blockers | Someone mentions one | Capture and assign |
| Close on time | 15 min mark | "That's time, parking lot after" |
| Assign follow-ups | End | "Sarah owns the build issue" |

## Your Stand-up Configuration

| Element | Your Choice |
|---------|-------------|
| **Format** | Round-Robin / Walk-Board / Exception / Async |
| **Time** | |
| **Duration** | |
| **Facilitator** | Rotating / Fixed: _________ |
| **Absent Protocol** | Async post required / Slack update / 1:1 later |
| **Parking Lot Location** | |

## Checklist

- [ ] Stand-up format selected
- [ ] Time and duration set
- [ ] Facilitator approach decided
- [ ] Absent protocol defined
- [ ] Parking lot process in place
- [ ] Team trained on anti-patterns
- [ ] Calendar invite sent

## Tasks

1. **Choose your format** based on team size and style
2. **Set consistent time** that works for all timezones
3. **Define facilitation** — rotating or fixed
4. **Try it for a week** — get feedback
5. **Adjust based on feedback**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.7 Async Communication Standards

## Why It Matters

Not everyone is online at the same time. Async communication enables deep work, timezone flexibility, and documented decisions. But without standards, messages get lost, context is missing, and urgent items wait while trivial ones interrupt. Async standards create clarity about when, where, and how to communicate.

## Framework: Communication Channel Matrix

| Channel | Use For | Response Time | Examples |
|---------|---------|---------------|----------|
| **Instant Message** | Quick questions, urgent issues | <1 hour (work hours) | "Is the build working?" |
| **Team Channel** | Announcements, discussions | <4 hours | "Sprint review moved to 3pm" |
| **Email** | External, formal, long-form | <24 hours | Vendor communication |
| **Document** | Decisions, specs, documentation | N/A (reference) | Design docs, decisions |
| **Tracking System** | Tasks, bugs, work items | <24 hours | "Bug assigned to you" |
| **Meeting** | Complex discussion, decisions | Scheduled | Design reviews |

```
┌─────────────────────────────────────────────────────────────────────┐
│              COMMUNICATION URGENCY MATRIX                           │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                        More Urgent                                  │
│                            │                                        │
│               Phone Call   │                                        │
│                  ▲         │                                        │
│               Video Call   │                                        │
│                  ▲         │                                        │
│            Instant Message │                                        │
│                  ▲         │                                        │
│             Team Channel   │                                        │
│                  ▲         │                                        │
│                Email       │                                        │
│                  ▲         │                                        │
│               Document     │                                        │
│                            │                                        │
│                        Less Urgent                                  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Channel Standards

### Slack/Chat Standards

| Element | Standard |
|---------|----------|
| **Channel naming** | #proj-[project]-[topic] |
| **Thread use** | Always thread for replies |
| **@mentions** | @channel for urgent, @person for specific |
| **Status** | Set when unavailable/focusing |
| **Response expectation** | Same business day |
| **After hours** | Schedule messages for morning |

### Email Standards

| Element | Standard |
|---------|----------|
| **Subject** | [Project] Action-oriented subject |
| **TL;DR** | First line summarizes |
| **Action items** | Bold or call out explicitly |
| **Recipients** | To: action required, CC: FYI only |
| **Response time** | 24 hours acknowledgment |
| **Threads** | Reply-all only when necessary |

### Document Standards

| Element | Standard |
|---------|----------|
| **Location** | Shared drive, consistent folder structure |
| **Naming** | [Project]-[Type]-[Topic]-[Date] |
| **Ownership** | Author listed, kept updated |
| **Status** | Draft / In Review / Final |
| **Comments** | Use comments, don't edit others' text |
| **Version** | Note significant changes |

## Framework: Message Quality Standards

### Good Async Message

```
Subject: [ACTION NEEDED] Character balance review - feedback by Friday

TL;DR: Please review attached balance changes and comment by EOD Friday.

Context:
- We're adjusting Tank characters based on playtest feedback
- Changes affect 3 characters (details in doc)

What I need:
- Your feedback on the attached spreadsheet
- Concerns about PvP implications
- Timeline conflicts if you can't review by Friday

Link: [Balance Doc]

Thanks!
```

### Poor Async Message

```
hey can someone look at this when they get a chance
[link]
thanks
```

## Framework: Async Message Template

```
Subject: [TYPE] Topic - [deadline if any]

TL;DR: One sentence summary

Context:
- Why this matters
- Background needed

Request:
- Specific action needed
- By when
- From whom (if specific)

Links/Attachments:
- [Relevant resources]
```

**Message Types:**
- [FYI] — No action needed
- [ACTION] — Action required
- [DECISION] — Decision needed
- [REVIEW] — Review requested
- [QUESTION] — Question to answer
- [URGENT] — Time-sensitive

## Framework: Response Expectations

| Sender | Expectation to Set |
|--------|-------------------|
| If you need response by specific time | State deadline clearly |
| If FYI only | Say "No response needed" |
| If you need acknowledgment | Ask for thumbs-up or reply |
| If complex topic | Offer to schedule call instead |

| Recipient | Expectation to Meet |
|-----------|---------------------|
| Can't respond fully yet | Acknowledge + give ETA |
| Need more information | Ask clarifying questions |
| Passed along to someone | Let sender know |
| Done/completed | Confirm closure |

## Framework: "No Meeting" Communication

When a meeting might not be needed:

| Instead of Meeting | Use Async |
|-------------------|-----------|
| Status update | Post in channel |
| Simple decision | Poll or thread |
| Document review | Comment in doc |
| Brainstorm | Async idea collection, then meeting |
| Announcement | Channel post |

## Checklist

- [ ] Channel purposes defined
- [ ] Response time expectations set
- [ ] Message quality standards documented
- [ ] Team aligned on conventions
- [ ] Channel naming consistent
- [ ] Urgent escalation path clear
- [ ] Focus time respected

## Tasks

1. **Define your channels** and their purposes
2. **Set response expectations** for each channel
3. **Create message templates** for common types
4. **Train team** on standards
5. **Audit periodically** — are standards followed?

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.8 Cross-Functional Data Sharing

## Why It Matters

Data is useless locked in silos. Analytics knows retention is dropping, but Design doesn't know which feature to fix. Marketing sees CPI rising, but Product doesn't know positioning needs change. Cross-functional data sharing turns information into action by getting the right data to the right people at the right time.

## Framework: Data Consumer Map

| Team | Key Data Needs | Current Source | Format | Frequency |
|------|----------------|----------------|--------|-----------|
| **Game Design** | Funnel data, feature usage, progression | | | |
| **Engineering** | Performance, crashes, errors | | | |
| **Art** | Load times, asset performance | | | |
| **QA** | Bug trends, regression data | | | |
| **Marketing** | CPI, ROAS, organic %, store metrics | | | |
| **Product** | Retention, LTV, engagement | | | |
| **Live Ops** | Event performance, offer conversion | | | |
| **Leadership** | KPIs, revenue, health summary | | | |

## Framework: Data Sharing Mechanisms

| Mechanism | Best For | Update Frequency | Effort |
|-----------|----------|-----------------|--------|
| **Automated Dashboard** | Regular KPIs | Real-time to daily | High setup, low ongoing |
| **Regular Report** | Periodic summary | Weekly/monthly | Medium |
| **Ad-Hoc Query** | Specific questions | On request | Low setup, per-request |
| **Alert** | Anomaly detection | Real-time | Medium |
| **Data Review Meeting** | Discussion of trends | Weekly | Low |

```
┌─────────────────────────────────────────────────────────────────────┐
│                    DATA SHARING ARCHITECTURE                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │                    DATA SOURCES                               │  │
│  │   Analytics    Server Logs    Store Data    Support Tickets   │  │
│  └─────────────────────────────┬─────────────────────────────────┘  │
│                                │                                    │
│                                ▼                                    │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │                    PROCESSING LAYER                           │  │
│  │        ETL / Data Warehouse / Analytics Platform              │  │
│  └─────────────────────────────┬─────────────────────────────────┘  │
│                                │                                    │
│          ┌─────────────────────┼─────────────────────┐              │
│          │                     │                     │              │
│          ▼                     ▼                     ▼              │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐     │
│  │   DASHBOARDS    │  │    REPORTS      │  │    ALERTS       │     │
│  │   Self-serve    │  │   Pushed to     │  │   Anomaly       │     │
│  │   exploration   │  │   stakeholders  │  │   detection     │     │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Dashboard Catalog

| Dashboard | Audience | Key Metrics | Access | Update |
|-----------|----------|-------------|--------|--------|
| **Executive Summary** | Leadership | Revenue, DAU, retention | Exec team | Daily |
| **Product Health** | Product, Design | Funnels, feature usage | Core team | Daily |
| **Live Ops** | Live Ops, Product | Event metrics, offers | Live team | Real-time |
| **Technical** | Engineering | Crashes, performance | Engineering | Real-time |
| **UA/Marketing** | Marketing | CPI, ROAS, organic | Marketing | Daily |
| **Economy** | Economy, Product | Currency flow, pricing | Core team | Daily |

## Framework: Regular Report Cadence

| Report | Frequency | Audience | Owner | Contents |
|--------|-----------|----------|-------|----------|
| **Daily Health** | Daily | Core team | Analytics | DAU, revenue, issues |
| **Weekly Digest** | Weekly | All | Analytics | Week summary, trends |
| **Sprint Metrics** | Per sprint | Team | Product | Feature performance |
| **Monthly Business** | Monthly | Leadership | Analytics | Full business review |
| **Event Post-Mortem** | Per event | Live Ops | Live Ops | Event performance |

## Framework: Data Review Meeting

| Element | Specification |
|---------|---------------|
| **Frequency** | Weekly |
| **Duration** | 30-45 minutes |
| **Attendees** | Product, Design, Analytics, Live Ops |
| **Facilitator** | Analytics |

**Agenda:**
1. Health check (5 min) — Are we green/yellow/red?
2. Key metrics review (10 min) — What moved?
3. Deep dive (15 min) — One topic in depth
4. Questions (5 min) — Team asks analytics
5. Actions (5 min) — What do we do with this?

## Framework: Self-Service Data Access

| User Level | Access | Training Needed |
|------------|--------|-----------------|
| **Basic** | Pre-built dashboards | 30-min overview |
| **Intermediate** | Dashboard filters, date ranges | 1-hour training |
| **Advanced** | Custom queries, exploration | Ongoing support |
| **Expert** | Raw data, custom analysis | Data team partnership |

## Framework: Data Request Process

For ad-hoc requests:

| Step | Owner | Timeline |
|------|-------|----------|
| Submit request | Requester | — |
| Triage and scope | Analytics | <1 day |
| Prioritize | Analytics + Product | <1 day |
| Execute | Analytics | Varies |
| Deliver and review | Analytics + Requester | — |

### Request Template

```
Data Request: [Title]
Requester: [Name]
Priority: Low / Medium / High / Urgent
Due Date: [If any]

Question to Answer:
[What are you trying to learn?]

How will you use this:
[What decision will this inform?]

Specific Metrics Needed:
- [Metric 1]
- [Metric 2]

Filters/Segments:
- [Date range]
- [User segments]
- [Other filters]
```

## Checklist

- [ ] Data consumers identified with needs
- [ ] Dashboard catalog created
- [ ] Regular reports scheduled
- [ ] Data review meeting established
- [ ] Self-service access tiered appropriately
- [ ] Request process defined
- [ ] Data team capacity planned

## Tasks

1. **Map data consumers** to their needs
2. **Inventory existing dashboards** and gaps
3. **Define regular report cadence**
4. **Establish weekly data review meeting**
5. **Create request intake process**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.9 Vendor & Partner Management

## Why It Matters

Modern games depend on external partners: ad networks, analytics SDKs, audio middleware, platform partners, outsourcing studios. Each relationship needs management—contracts, contacts, escalation paths, integration support. Vendor chaos creates project risk; vendor management creates reliability.

## Framework: Vendor Inventory

| Vendor | Category | Service | Contract End | Key Contact | Internal Owner |
|--------|----------|---------|--------------|-------------|----------------|
| | Analytics | | | | |
| | Attribution | | | | |
| | Ads | | | | |
| | Server/Backend | | | | |
| | Crash Reporting | | | | |
| | Localization | | | | |
| | Audio | | | | |
| | Art Outsource | | | | |
| | QA Outsource | | | | |
| | Platform (Apple) | | | | |
| | Platform (Google) | | | | |

## Framework: Vendor Relationship Tiers

| Tier | Criteria | Management Level | Review Frequency |
|------|----------|------------------|------------------|
| **Critical** | Game doesn't work without them | Executive relationship | Monthly |
| **Important** | Significant impact if fails | Lead relationship | Quarterly |
| **Standard** | Useful, replaceable | Working relationship | Annually |
| **Commodity** | Interchangeable, low impact | Contract only | As needed |

### Tier Assessment

| Vendor | Dependency Level | Replaceability | Business Impact | Tier |
|--------|------------------|----------------|-----------------|------|
| | High/Med/Low | Easy/Mod/Hard | High/Med/Low | |
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Vendor Contact Matrix

| Vendor | Sales Contact | Technical Contact | Support Contact | Escalation Contact |
|--------|---------------|-------------------|-----------------|-------------------|
| | | | | |
| | | | | |
| | | | | |
| | | | | |

## Framework: Vendor Onboarding Checklist

When adding a new vendor:

- [ ] Contract reviewed and signed
- [ ] NDA in place (if needed)
- [ ] Internal owner assigned
- [ ] Key contacts identified
- [ ] Support channels established
- [ ] SLA understood
- [ ] Integration documentation obtained
- [ ] Test environment provided
- [ ] Escalation path confirmed
- [ ] Billing setup complete
- [ ] Added to vendor inventory

## Framework: Vendor Health Monitoring

| Vendor | SLA Metric | Target | Current | Trend | Action Needed |
|--------|------------|--------|---------|-------|---------------|
| | Uptime | | | ↑↓→ | |
| | Response Time | | | ↑↓→ | |
| | Issue Resolution | | | ↑↓→ | |
| | | | | | |
| | | | | | |

## Framework: Vendor Communication Rhythm

| Tier | Meeting Frequency | Attendees | Agenda |
|------|-------------------|-----------|--------|
| **Critical** | Monthly | Exec + Lead | Performance, roadmap, relationship |
| **Important** | Quarterly | Lead + Technical | Performance, integration, issues |
| **Standard** | Annually | Lead | Contract review, performance |
| **Commodity** | As needed | Owner | Issues only |

## Framework: Vendor Issue Escalation

| Severity | First Contact | Response Target | Escalate If |
|----------|---------------|-----------------|-------------|
| Critical | Support + Account | <1 hour | No response 1 hour |
| High | Support | <4 hours | No response 4 hours |
| Medium | Support | <24 hours | No response 24 hours |
| Low | Support | <72 hours | Pattern of issues |

### Escalation Path

```
Support → Account Manager → Regional Manager → Executive Sponsor
```

## Framework: Vendor Risk Assessment

| Vendor | Risk | Likelihood | Impact | Mitigation |
|--------|------|------------|--------|------------|
| | Service shutdown | | | Backup plan |
| | Price increase | | | Contract terms |
| | API deprecation | | | Version monitoring |
| | Acquisition/change | | | Relationship |
| | Performance issue | | | SLA enforcement |

## Checklist

- [ ] All vendors inventoried
- [ ] Tiers assigned
- [ ] Contacts documented
- [ ] Internal owners assigned
- [ ] SLAs understood
- [ ] Escalation paths clear
- [ ] Meeting rhythm established
- [ ] Risks assessed

## Tasks

1. **Inventory all vendors** and services
2. **Assign tiers** based on criticality
3. **Document contacts** and escalation
4. **Assign internal owners** for each vendor
5. **Establish meeting rhythm** for critical vendors

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.10 On-Call & Coverage Rotation

## Why It Matters

Games don't stop running at 5pm. Events launch on weekends. Server issues happen at 3am. Without on-call coverage, problems wait until Monday—losing revenue and player trust. But on-call without rotation leads to burnout. A structured rotation ensures coverage while protecting team wellbeing.

## Framework: Coverage Requirements

| Coverage Type | When Needed | Severity | Response Time |
|---------------|-------------|----------|---------------|
| **Critical** | 24/7 | Game down, data loss | <15 min |
| **High** | Extended hours | Major issues | <1 hour |
| **Standard** | Business hours | Normal issues | <4 hours |
| **Planned** | Events, launches | Event-specific | Active monitoring |

## Framework: On-Call Tiers

```
┌─────────────────────────────────────────────────────────────────────┐
│                      ON-CALL STRUCTURE                              │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │                    TIER 1: First Response                   │    │
│  │  • Check if real issue                                      │    │
│  │  • Apply known fixes                                        │    │
│  │  • Escalate if needed                                       │    │
│  │  Response: <15 min                                          │    │
│  └─────────────────────────────┬───────────────────────────────┘    │
│                                │ Escalate                           │
│                                ▼                                    │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │                    TIER 2: Engineering                      │    │
│  │  • Diagnose complex issues                                  │    │
│  │  • Implement fixes                                          │    │
│  │  • Coordinate war room if needed                            │    │
│  │  Response: <30 min                                          │    │
│  └─────────────────────────────┬───────────────────────────────┘    │
│                                │ Escalate                           │
│                                ▼                                    │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │                    TIER 3: Leadership                       │    │
│  │  • Major decisions                                          │    │
│  │  • External communication                                   │    │
│  │  • Resource allocation                                      │    │
│  │  Response: <1 hour                                          │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Rotation Schedule

### Weekly Rotation Template

| Week | Tier 1 Primary | Tier 1 Backup | Tier 2 | Tier 3 |
|------|----------------|---------------|--------|--------|
| Week 1 | | | | |
| Week 2 | | | | |
| Week 3 | | | | |
| Week 4 | | | | |

### Monthly Calendar

| Role | Week 1 | Week 2 | Week 3 | Week 4 |
|------|--------|--------|--------|--------|
| Person A | On-call | Off | Off | Backup |
| Person B | Backup | On-call | Off | Off |
| Person C | Off | Backup | On-call | Off |
| Person D | Off | Off | Backup | On-call |

**Rotation Rules:**
- Minimum 3-4 people in rotation
- No back-to-back weeks
- Maximum 1 week on-call per month
- Swap policy for conflicts

## Framework: On-Call Expectations

| Expectation | Specification |
|-------------|---------------|
| **Response time** | Acknowledge alert within 15 minutes |
| **Availability** | Phone accessible, internet access |
| **Sobriety** | Alert and capable of working |
| **Location** | Within 1 hour of workstation |
| **Handoff** | Briefing when rotation changes |
| **Documentation** | Log all incidents |

## Framework: On-Call Compensation

| Compensation Type | Description |
|-------------------|-------------|
| **Time-off in lieu** | Hour for hour compensation time |
| **Flat rate** | Fixed amount per on-call shift |
| **Incident-based** | Additional pay per incident |
| **Premium rate** | Higher hourly rate for after-hours |
| **Rotation bonus** | Monthly/quarterly bonus for participants |

**Your Policy:** _______________________

## Framework: On-Call Toolkit

| Tool | Purpose | Access Verified |
|------|---------|-----------------|
| Paging/alerting system | Receive alerts | ☐ |
| Runbooks | Step-by-step responses | ☐ |
| Admin access | Make changes | ☐ |
| Monitoring dashboards | See status | ☐ |
| Communication channel | Coordinate response | ☐ |
| Escalation contacts | Reach backup | ☐ |
| VPN/remote access | Access systems | ☐ |

## Framework: Handoff Protocol

### End of Shift Handoff

```
On-Call Handoff: [Date]

Outgoing: [Name]
Incoming: [Name]

Active Issues:
- [Issue 1]: [Status]
- [Issue 2]: [Status]

Things to Watch:
- [Event launching Friday]
- [Build deploying Monday]

Notes:
- [Any context]
```

## Framework: On-Call Health Metrics

| Metric | Target | Current | Trend |
|--------|--------|---------|-------|
| Incidents per week | | | ↑↓→ |
| Average response time | <15 min | | ↑↓→ |
| Escalation rate | <20% | | ↑↓→ |
| Mean time to resolve | | | ↑↓→ |
| After-hours incidents | Decreasing | | ↑↓→ |

## Checklist

- [ ] Coverage requirements defined
- [ ] On-call tiers established
- [ ] Rotation schedule created
- [ ] Expectations documented
- [ ] Compensation policy set
- [ ] Toolkit verified for all participants
- [ ] Handoff protocol defined
- [ ] Health metrics tracked

## Tasks

1. **Define coverage requirements** for your game
2. **Create rotation schedule** with minimum team
3. **Document expectations** clearly
4. **Establish compensation policy**
5. **Test the system** with a drill

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.11 Feedback Loop Architecture

## Why It Matters

Feedback from players is gold—but only if it reaches the right people and drives action. A broken feedback loop means designers guess instead of know, support issues don't prevent product problems, and players feel unheard. Feedback architecture ensures signals flow from players to decisions and back.

## Framework: Feedback Flow

```
┌─────────────────────────────────────────────────────────────────────┐
│                      FEEDBACK FLOW ARCHITECTURE                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                         ┌───────────────┐                           │
│                         │    PLAYERS    │                           │
│                         └───────┬───────┘                           │
│                                 │                                   │
│    ┌────────────────────────────┼────────────────────────────┐      │
│    │                            │                            │      │
│    ▼                            ▼                            ▼      │
│ ┌──────────┐            ┌──────────────┐            ┌──────────┐   │
│ │ REVIEWS  │            │   SOCIAL /   │            │ SUPPORT  │   │
│ │          │            │  COMMUNITY   │            │ TICKETS  │   │
│ │ App Store│            │              │            │          │   │
│ │ Ratings  │            │ Discord,     │            │ Bug      │   │
│ │          │            │ Reddit,      │            │ reports, │   │
│ │          │            │ Forums       │            │ issues   │   │
│ └────┬─────┘            └──────┬───────┘            └────┬─────┘   │
│      │                         │                         │         │
│      └─────────────────────────┼─────────────────────────┘         │
│                                │                                    │
│                                ▼                                    │
│                       ┌────────────────┐                            │
│                       │  AGGREGATION   │                            │
│                       │  & ANALYSIS    │                            │
│                       │                │                            │
│                       │ Community team │                            │
│                       │ aggregates,    │                            │
│                       │ categorizes,   │                            │
│                       │ prioritizes    │                            │
│                       └────────┬───────┘                            │
│                                │                                    │
│                                ▼                                    │
│                       ┌────────────────┐                            │
│                       │   PRODUCT      │                            │
│                       │   DECISIONS    │                            │
│                       └────────┬───────┘                            │
│                                │                                    │
│                                ▼                                    │
│                       ┌────────────────┐                            │
│                       │  COMMUNICATE   │                            │
│                       │  BACK          │                            │
│                       │                │                            │
│                       │ Patch notes,   │                            │
│                       │ responses,     │                            │
│                       │ updates        │                            │
│                       └────────────────┘                            │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Feedback Source Matrix

| Source | Signal Type | Volume | Quality | Owner | Frequency Check |
|--------|-------------|--------|---------|-------|-----------------|
| App Store Reviews | Sentiment, issues | High | Medium | Community | Daily |
| Social Media | Sentiment, trends | High | Low | Community | Continuous |
| Discord/Forums | Detailed feedback | Medium | High | Community | Daily |
| Support Tickets | Issues, bugs | Medium | High | Support | Daily |
| Survey Responses | Targeted questions | Low | Very High | Product | Per survey |
| Playtest Sessions | Behavior, verbal | Low | Very High | Design | Per session |
| Analytics | Behavior | Very High | High | Analytics | Daily |
| Churn Surveys | Exit reasons | Low | High | Product | Continuous |

## Framework: Feedback Categorization

| Category | Examples | Routing |
|----------|----------|---------|
| **Bug Report** | Crashes, errors, glitches | QA → Engineering |
| **Feature Request** | New ideas, additions | Product backlog |
| **Balance Complaint** | Too hard, too easy, unfair | Design |
| **Monetization Complaint** | Prices, value, P2W | Economy Design |
| **Content Request** | More levels, characters | Content roadmap |
| **UX Issue** | Confusing UI, poor flow | UX Design |
| **Technical Issue** | Performance, loading | Engineering |
| **Positive Feedback** | Appreciation | Team morale |

## Framework: Feedback Aggregation Report

### Weekly Feedback Summary Template

```
Week of: [Date]

Volume:
- Reviews: [count], Avg rating: [stars]
- Support tickets: [count], Resolution: [%]
- Social mentions: [count], Sentiment: [%pos/%neg]

Top Themes (by volume):
1. [Theme] - [count] mentions - [Trend ↑↓→]
2. [Theme] - [count] mentions - [Trend ↑↓→]
3. [Theme] - [count] mentions - [Trend ↑↓→]

Emerging Issues:
- [New issue appearing]

Positive Highlights:
- [What players love]

Recommended Actions:
- [Action 1] - [Priority]
- [Action 2] - [Priority]
```

## Framework: Feedback → Action Process

| Step | Owner | Output |
|------|-------|--------|
| 1. Collect | Community | Raw feedback gathered |
| 2. Categorize | Community | Feedback sorted by type |
| 3. Aggregate | Community | Summary with trends |
| 4. Analyze | Product + Design | Insights identified |
| 5. Prioritize | Product | Actions ranked |
| 6. Plan | Product + Team | Work scheduled |
| 7. Execute | Team | Changes made |
| 8. Communicate | Community | Players informed |

## Framework: Closing the Loop

| Feedback Type | Response |
|---------------|----------|
| Bug fixed | Patch notes mention |
| Feature added | Announcement |
| Request declined | Explanation (sometimes) |
| General improvement | Update notes |
| Major change | Community post |

### Communication Templates

**When fixed:**
```
Many of you reported [issue]. We've fixed this in version [X]. Thank you for your feedback!
```

**When adding requested feature:**
```
You asked, we listened! [Feature] is coming in [update]. Thanks for the suggestion!
```

**When not fixing:**
```
We've heard your feedback on [topic]. After consideration, we've decided to [approach] because [reason]. We know this isn't what everyone hoped for, and we'll continue to monitor.
```

## Framework: Feedback Health Metrics

| Metric | Target | Current | Trend |
|--------|--------|---------|-------|
| Review response rate | >20% | | ↑↓→ |
| Avg rating | >4.0 | | ↑↓→ |
| Support resolution time | <24h | | ↑↓→ |
| Player sentiment | >60% positive | | ↑↓→ |
| Feedback → Action cycle | <4 weeks | | ↑↓→ |

## Checklist

- [ ] Feedback sources identified
- [ ] Ownership assigned per source
- [ ] Categorization system defined
- [ ] Aggregation process established
- [ ] Routing to teams clear
- [ ] Action prioritization process set
- [ ] Communication back process defined
- [ ] Health metrics tracked

## Tasks

1. **Inventory feedback sources** and assign owners
2. **Create categorization system** for your game
3. **Establish weekly summary process**
4. **Define feedback → action workflow**
5. **Plan communication-back strategy**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.12 Onboarding Checklist

## Why It Matters

New team members take weeks to become productive—longer without good onboarding. That's expensive time and risks early frustration or departure. A comprehensive onboarding checklist ensures new hires get the access, context, and relationships they need to contribute quickly.

## Framework: Onboarding Phases

```
┌─────────────────────────────────────────────────────────────────────┐
│                      ONBOARDING JOURNEY                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  BEFORE DAY 1          DAY 1           WEEK 1          MONTH 1     │
│  ┌──────────┐      ┌──────────┐      ┌──────────┐    ┌──────────┐  │
│  │ PREPARE  │─────▶│ WELCOME  │─────▶│  LEARN   │───▶│CONTRIBUTE│  │
│  │          │      │          │      │          │    │          │  │
│  │ Systems  │      │ Context  │      │ Deep dive│    │ First    │  │
│  │ ready    │      │ setting  │      │ into work│    │ impact   │  │
│  └──────────┘      └──────────┘      └──────────┘    └──────────┘  │
│                                                                     │
│                          ONGOING                                    │
│                      ┌──────────┐                                   │
│                      │  GROW    │                                   │
│                      │          │                                   │
│                      │ Feedback │                                   │
│                      │ & growth │                                   │
│                      └──────────┘                                   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Pre-Day 1 Checklist

**Completed by: Manager + HR + IT**

### Access & Accounts
- [ ] Email account created
- [ ] Slack/chat access provisioned
- [ ] Project tracking tool access (Jira, etc.)
- [ ] Document drive access
- [ ] Source control access (if applicable)
- [ ] Build system access (if applicable)
- [ ] Game dev environment set up
- [ ] VPN configured (if remote)
- [ ] Analytics dashboard access

### Hardware & Setup
- [ ] Computer/laptop ready
- [ ] Monitors, peripherals
- [ ] Dev kit access (if applicable)
- [ ] Software licenses provisioned

### Documentation Ready
- [ ] Onboarding doc prepared
- [ ] Team org chart current
- [ ] Project documentation accessible
- [ ] Meeting invites sent

### People Prep
- [ ] Manager notified
- [ ] Team notified of start date
- [ ] Onboarding buddy assigned
- [ ] 1:1s scheduled with key people

## Framework: Day 1 Checklist

### Morning

- [ ] Warm welcome from manager
- [ ] Desk/equipment check
- [ ] Account access verified
- [ ] HR paperwork completed
- [ ] Team introduction

### Afternoon

- [ ] Project overview (30-60 min with manager)
- [ ] Game walkthrough (play the game!)
- [ ] Development environment setup
- [ ] First 1:1 with manager (goals, expectations)
- [ ] Onboarding buddy check-in

### End of Day

- [ ] Questions answered
- [ ] Tomorrow's plan clear
- [ ] Knows who to contact for help

## Framework: Week 1 Checklist

### Understanding the Project
- [ ] Read vision document
- [ ] Read project pillars
- [ ] Understand current milestone
- [ ] Review scope document
- [ ] Play the game for 2+ hours
- [ ] Review competitor games

### Meeting the Team
- [ ] 1:1 with each direct team member (15-30 min each)
- [ ] Meet cross-functional partners
- [ ] Understand team structure and roles
- [ ] Attend key team meetings

### Getting Productive
- [ ] Complete first small task
- [ ] Navigate codebase/tools successfully
- [ ] Ask questions (many!)
- [ ] Document confusion points (helps improve onboarding)

### Learning Systems
- [ ] Build system walkthrough
- [ ] Deployment process overview
- [ ] Analytics tools introduction
- [ ] Bug tracking workflow

## Framework: Month 1 Checklist

### Contribution
- [ ] Complete 2-3 meaningful tasks
- [ ] Participate in sprint planning
- [ ] Provide input in design discussions
- [ ] Create/update documentation

### Integration
- [ ] Comfortable asking anyone questions
- [ ] Understands team norms and culture
- [ ] Can navigate tools independently
- [ ] Attends and contributes to meetings

### Feedback
- [ ] 30-day check-in with manager
- [ ] Share onboarding feedback
- [ ] Goals for next 60 days set
- [ ] Identify learning priorities

## Framework: Onboarding Buddy Role

| Buddy Responsibility | Details |
|---------------------|---------|
| Daily check-in (Week 1) | 15 min: questions, blockers |
| Weekly check-in (Month 1) | 30 min: deeper questions |
| Answer "dumb" questions | Create safe space to ask |
| Introduce to others | Help build network |
| Share unwritten rules | Culture, norms, tips |
| Escalate issues | Flag to manager if stuck |

## Framework: Role-Specific Additions

### Designer Onboarding Add-ons
- [ ] Design tool walkthroughs
- [ ] Design doc standards
- [ ] Playtest process overview
- [ ] Economy docs review

### Engineer Onboarding Add-ons
- [ ] Architecture walkthrough
- [ ] Code review standards
- [ ] Build and deploy process
- [ ] On-call introduction

### Artist Onboarding Add-ons
- [ ] Art bible review
- [ ] Asset pipeline walkthrough
- [ ] Naming conventions
- [ ] Export specifications

### Producer Onboarding Add-ons
- [ ] Current roadmap and timeline
- [ ] Stakeholder introductions
- [ ] Reporting requirements
- [ ] Meeting ownership

## Checklist

- [ ] Pre-Day 1 checklist completed
- [ ] Day 1 agenda prepared
- [ ] Week 1 plan defined
- [ ] Month 1 milestones set
- [ ] Onboarding buddy assigned and briefed
- [ ] Role-specific additions identified
- [ ] Feedback collection scheduled
- [ ] Onboarding template maintained and improved

## Tasks

1. **Create onboarding template** for your team
2. **Assign onboarding buddy** role formally
3. **Prepare before each new hire** using checklist
4. **Collect feedback** from recent hires
5. **Iterate and improve** the process

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.13 Knowledge Base Maintenance

## Why It Matters

Knowledge walks out the door with every departure. Decisions made months ago become mysteries. New hires reinvent solved problems. A maintained knowledge base preserves institutional memory, enables self-service answers, and reduces "ask Sarah, she knows" bottlenecks.

## Framework: Knowledge Base Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                    KNOWLEDGE BASE STRUCTURE                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  📁 PROJECT                                                         │
│  ├── 📄 Vision & Pillars                                            │
│  ├── 📄 Scope Document                                              │
│  ├── 📄 Timeline & Milestones                                       │
│  └── 📄 Team & Contacts                                             │
│                                                                     │
│  📁 DESIGN                                                          │
│  ├── 📄 Game Design Document                                        │
│  ├── 📄 Feature Specs                                               │
│  ├── 📄 Economy Design                                              │
│  ├── 📄 Balance Data                                                │
│  └── 📄 Content Guidelines                                          │
│                                                                     │
│  📁 TECHNICAL                                                       │
│  ├── 📄 Architecture Overview                                       │
│  ├── 📄 Setup Instructions                                          │
│  ├── 📄 Coding Standards                                            │
│  ├── 📄 API Documentation                                           │
│  └── 📄 Runbooks                                                    │
│                                                                     │
│  📁 ART                                                             │
│  ├── 📄 Art Bible                                                   │
│  ├── 📄 Asset Pipeline                                              │
│  └── 📄 Style Guides                                                │
│                                                                     │
│  📁 OPERATIONS                                                      │
│  ├── 📄 Release Process                                             │
│  ├── 📄 Incident Response                                           │
│  ├── 📄 On-Call Procedures                                          │
│  └── 📄 Vendor Information                                          │
│                                                                     │
│  📁 DECISIONS                                                       │
│  ├── 📄 Decision Log                                                │
│  └── 📄 Post-Mortems                                                │
│                                                                     │
│  📁 PROCESSES                                                       │
│  ├── 📄 Onboarding                                                  │
│  ├── 📄 Meeting Guides                                              │
│  └── 📄 How-To Guides                                               │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Document Types

| Type | Purpose | Update Frequency | Owner |
|------|---------|------------------|-------|
| **Reference** | Stable information, standards | Quarterly review | Domain lead |
| **Specification** | Feature/system details | Per feature | Author |
| **Process** | How to do things | When process changes | Process owner |
| **Decision** | Why choices were made | When decisions made | Decision maker |
| **Runbook** | Step-by-step procedures | When procedure changes | Operations |
| **Guide** | Teaching/onboarding | As needed | Various |

## Framework: Document Template

```
# [Document Title]

**Owner:** [Name]
**Last Updated:** [Date]
**Status:** Draft / In Review / Current / Archived

## Summary
[2-3 sentences: what is this and who is it for]

## Content
[Main content]

## Related Documents
- [Link 1]
- [Link 2]

## Changelog
| Date | Author | Change |
|------|--------|--------|
| | | |
```

## Framework: Maintenance Rhythm

| Frequency | Activity | Owner |
|-----------|----------|-------|
| **Weekly** | Check for broken links | Anyone (report) |
| **Monthly** | Review recently changed docs | Doc owners |
| **Quarterly** | Audit all docs for accuracy | Team leads |
| **Per milestone** | Update project docs | Producer |
| **Per decision** | Log significant decisions | Decision maker |
| **Per incident** | Write/update runbook | Responders |

## Framework: Knowledge Capture Triggers

| Trigger | Document to Create/Update |
|---------|--------------------------|
| New team member asks same question 3x | FAQ or How-To guide |
| Decision with multiple stakeholders | Decision log entry |
| Process confusion or errors | Process documentation |
| Incident occurred | Runbook update |
| Feature shipped | Feature spec finalized |
| Major milestone | Project docs updated |
| Team member leaving | Knowledge transfer session |

## Framework: Documentation Health Metrics

| Metric | Target | How to Measure |
|--------|--------|----------------|
| Docs with owners | 100% | Audit |
| Docs updated in 6 months | >80% | Last modified date |
| Onboarding satisfaction | >4/5 | Survey |
| Time to find information | <5 min | Survey |
| Broken links | 0 | Automated check |

## Framework: Knowledge Base Audit Checklist

### Quarterly Audit

For each document:
- [ ] Owner still valid?
- [ ] Content still accurate?
- [ ] Still needed?
- [ ] Links working?
- [ ] Properly categorized?

### Results Actions

| Finding | Action |
|---------|--------|
| Owner left | Reassign ownership |
| Content outdated | Update or archive |
| Not needed | Archive or delete |
| Links broken | Fix or remove |
| Hard to find | Recategorize, improve titles |

## Framework: Document Lifecycle

```
┌─────────┐    ┌──────────┐    ┌─────────┐    ┌──────────┐
│  DRAFT  │───▶│ IN REVIEW│───▶│ CURRENT │───▶│ ARCHIVED │
└─────────┘    └──────────┘    └─────────┘    └──────────┘
                                    │
                                    │ Update
                                    ▼
                               ┌─────────┐
                               │  DRAFT  │
                               │ (new ver│
                               └─────────┘
```

## Checklist

- [ ] Folder structure established
- [ ] Document templates created
- [ ] Ownership assigned
- [ ] Maintenance rhythm set
- [ ] Capture triggers defined
- [ ] Health metrics tracked
- [ ] Quarterly audit scheduled
- [ ] Team trained on knowledge base use

## Tasks

1. **Create folder structure** for your knowledge base
2. **Inventory existing documents** and migrate
3. **Assign owners** to all documents
4. **Create templates** for common doc types
5. **Schedule first quarterly audit**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.14 Conflict Resolution Framework

## Why It Matters

Conflict is inevitable when passionate people work together—especially at the intersection of creative, technical, and business priorities. Unresolved conflict festers into dysfunction; avoided conflict leads to poor decisions. A framework for healthy conflict resolution turns disagreements into better outcomes.

## Framework: Conflict Types in Game Development

| Conflict Type | Example | Root Cause |
|---------------|---------|------------|
| **Priority** | "My feature should ship first" | Limited resources |
| **Technical** | "My approach is better" | Different valid solutions |
| **Creative** | "The design should be X, not Y" | Subjective preferences |
| **Process** | "We should do it this way" | Different work styles |
| **Resource** | "I need more time/people" | Scarcity |
| **Values** | "This crosses an ethical line" | Fundamental beliefs |
| **Interpersonal** | "I don't trust their judgment" | Relationship damage |

## Framework: Conflict Escalation Ladder

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CONFLICT RESOLUTION LADDER                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  LEVEL 5: Executive Decision                                        │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │ Leadership makes final call, all parties accept              │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                              ▲                                      │
│                              │ Escalate if unresolved               │
│  LEVEL 4: Facilitated Discussion                                    │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │ Neutral third party facilitates, seeks compromise            │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                              ▲                                      │
│                              │ Escalate if unresolved               │
│  LEVEL 3: Manager Mediation                                         │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │ Shared manager helps find solution, may decide               │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                              ▲                                      │
│                              │ Escalate if unresolved               │
│  LEVEL 2: Structured 1:1                                            │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │ Parties meet with framework, seek mutual solution            │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                              ▲                                      │
│                              │ Escalate if unresolved               │
│  LEVEL 1: Direct Conversation                                       │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │ Address directly, assume good intent, seek understanding     │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                                                                     │
│  START HERE ───────────────────────────────────────────────────▶    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Conflict Resolution Conversation

### Preparation
1. **Identify the issue** — What specifically is the conflict about?
2. **Understand your goal** — What outcome do you need?
3. **Consider their perspective** — What might they want?
4. **Plan timing** — When and where to have the conversation?

### The Conversation

**Opening:**
- "I'd like to discuss [topic]. Is now a good time?"
- "I value our working relationship and want to address something"

**Structure:**
1. **State the issue** (observation, not accusation)
   - "I noticed..." not "You always..."
2. **Express impact** (your perspective)
   - "This affects me because..."
3. **Invite their perspective**
   - "Help me understand your view..."
4. **Seek shared ground**
   - "What do we both want here?"
5. **Propose solutions**
   - "What if we..."
6. **Agree on action**
   - "So we'll..."

### Closing
- Confirm understanding
- Agree on follow-up
- Express appreciation for the conversation

## Framework: Decision Framework for Conflicts

When parties can't agree, use decision rights:

| Question | If Yes | If No |
|----------|--------|-------|
| Does one party have decision authority? | They decide, other commits | Continue to next |
| Is there a tiebreaker role defined? | Engage tiebreaker | Continue to next |
| Can we try both and test? | Run experiment | Continue to next |
| Can we compromise? | Find middle ground | Continue to next |
| Is this blocking critical work? | Escalate to leadership | Continue discussion |

## Framework: "Disagree and Commit"

When decision is made that you disagreed with:

| Behavior | Required | Not Acceptable |
|----------|----------|----------------|
| Public support | ✓ | Undermining |
| Execution effort | ✓ | Sabotage |
| Monitoring results | ✓ | "Told you so" |
| Raising concerns appropriately | ✓ | Passive resistance |
| Revisiting if data changes | ✓ | Endless relitigating |

## Framework: Common Conflict Scenarios

### Scenario: Design vs. Engineering on Feasibility

| Step | Action |
|------|--------|
| 1 | Engineer explains technical constraints clearly |
| 2 | Designer explains design intent and goals |
| 3 | Both explore alternatives together |
| 4 | If stuck, escalate to Tech Lead + Design Lead |
| 5 | Final decision by whoever has domain authority |

### Scenario: Monetization vs. Player Experience

| Step | Action |
|------|--------|
| 1 | Monetization explains revenue goal |
| 2 | Design explains player experience concern |
| 3 | Review data on similar implementations |
| 4 | Explore alternatives that achieve both |
| 5 | If stuck, escalate to Product Lead with data |
| 6 | Test with A/B if possible |

### Scenario: Timeline vs. Quality

| Step | Action |
|------|--------|
| 1 | Producer explains timeline constraint |
| 2 | Team explains quality/scope concern |
| 3 | Identify minimum viable options |
| 4 | Assess risk of each option |
| 5 | Decision by whoever owns timeline |
| 6 | Document trade-off made |

## Framework: Conflict Prevention

| Practice | How It Helps |
|----------|--------------|
| Clear decision rights | Prevents "who decides" conflicts |
| Regular 1:1s | Surfaces issues early |
| Retrospectives | Addresses process conflicts |
| Shared goals | Aligns priorities |
| Assumption checking | Prevents misunderstandings |
| Psychological safety | Enables honest disagreement |

## Checklist

- [ ] Conflict types understood by team
- [ ] Escalation ladder defined
- [ ] Conversation framework shared
- [ ] Decision rights clear
- [ ] "Disagree and commit" norm established
- [ ] Common scenarios documented
- [ ] Prevention practices in place

## Tasks

1. **Share this framework** with your team
2. **Define your escalation ladder** with specific names
3. **Practice conflict conversations** in low-stakes situations
4. **Establish "disagree and commit" norm** explicitly
5. **Review after conflicts** — did the framework help?

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 3A.15 Team Health Pulse

## Why It Matters

Sustainable pace beats crunch. Burnout leads to turnover, quality problems, and long-term productivity loss. Regular team health checks surface issues before they become crises, show the team their wellbeing matters, and give leadership actionable data on team sustainability.

## Framework: Team Health Dimensions

```
┌─────────────────────────────────────────────────────────────────────┐
│                      TEAM HEALTH DIMENSIONS                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐              │
│  │   WORKLOAD   │  │  ENGAGEMENT  │  │   CLARITY    │              │
│  │              │  │              │  │              │              │
│  │ Sustainable? │  │ Motivated?   │  │ Direction    │              │
│  │ Balanced?    │  │ Enjoying     │  │ clear?       │              │
│  │ Predictable? │  │ work?        │  │ Priorities   │              │
│  │              │  │              │  │ understood?  │              │
│  └──────────────┘  └──────────────┘  └──────────────┘              │
│                                                                     │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐              │
│  │ COLLABORATION│  │   SUPPORT    │  │   GROWTH     │              │
│  │              │  │              │  │              │              │
│  │ Working well │  │ Supported    │  │ Learning?    │              │
│  │ together?    │  │ by manager?  │  │ Developing?  │              │
│  │ Communication│  │ Resources    │  │ Career path  │              │
│  │ healthy?     │  │ available?   │  │ visible?     │              │
│  └──────────────┘  └──────────────┘  └──────────────┘              │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Pulse Survey Template

**Frequency:** Weekly (light) or Bi-weekly (comprehensive)

### Quick Pulse (Weekly, 2 min)

```
1. How are you feeling about work this week? (1-5)
   1 = Struggling  |  5 = Great

2. Is your workload sustainable? (1-5)
   1 = Overwhelmed  |  5 = Comfortable

3. One word to describe the week: __________

4. Anything you want to flag? (optional)
   __________________________________________
```

### Comprehensive Pulse (Bi-weekly, 5 min)

| Dimension | Question | Scale |
|-----------|----------|-------|
| Workload | My workload is sustainable | 1-5 |
| Clarity | I understand priorities and expectations | 1-5 |
| Engagement | I'm motivated by my work | 1-5 |
| Collaboration | Team communication is healthy | 1-5 |
| Support | I have what I need to do my job | 1-5 |
| Growth | I'm learning and developing | 1-5 |

**Open-ended:**
- What's going well?
- What could be better?
- What support do you need?

## Framework: Health Metrics Dashboard

| Metric | Green | Yellow | Red | Current | Trend |
|--------|-------|--------|-----|---------|-------|
| Avg. workload score | >3.5 | 2.5-3.5 | <2.5 | | ↑↓→ |
| Avg. engagement | >3.5 | 2.5-3.5 | <2.5 | | ↑↓→ |
| Avg. clarity | >4.0 | 3.0-4.0 | <3.0 | | ↑↓→ |
| Survey response rate | >80% | 50-80% | <50% | | ↑↓→ |
| Overtime hours/week | <5 | 5-10 | >10 | | ↑↓→ |
| PTO utilization | >80% | 50-80% | <50% | | ↑↓→ |
| Voluntary turnover | <10%/yr | 10-20%/yr | >20%/yr | | ↑↓→ |

## Framework: Burnout Warning Signs

| Warning Sign | Observable Behavior | Action |
|--------------|---------------------|--------|
| Declining scores | 2+ weeks of dropping pulse scores | 1:1 check-in |
| Withdrawal | Less participation in meetings, chat | Direct conversation |
| Quality drop | More bugs, mistakes | Assess workload |
| Cynicism | Negative comments about project/company | Understand concerns |
| Exhaustion | Visible fatigue, sick days up | Enforce PTO |
| Overtime pattern | Consistently working late/weekends | Redistribute work |

## Framework: Response Protocol

| Health Status | Response |
|---------------|----------|
| **Green** (Healthy) | Maintain, recognize, don't add load |
| **Yellow** (Concerning) | Investigate, address specific concerns, monitor closely |
| **Red** (Critical) | Immediate intervention, redistribute work, enforce rest |

### Yellow Response Actions

- [ ] 1:1 with affected team members
- [ ] Identify root causes
- [ ] Create action plan with timeline
- [ ] Reduce non-essential work
- [ ] Communicate changes to team
- [ ] Monitor for improvement

### Red Response Actions

- [ ] Immediately reduce workload
- [ ] Cancel non-critical commitments
- [ ] Enforce time off if needed
- [ ] Leadership involvement
- [ ] External support if appropriate
- [ ] Post-crisis retrospective

## Framework: Sustainable Pace Guidelines

| Guideline | Standard |
|-----------|----------|
| Standard week | 40 hours |
| Maximum sustained | 45 hours |
| Crunch maximum | 50 hours (rare, time-limited) |
| Mandatory rest after crunch | Comp time or light week |
| Minimum PTO | Take all allocated time |
| Weekend work | Emergency only, always comped |
| Response outside hours | Not expected unless on-call |

## Framework: Team Health Retrospective

**Quarterly, 60 minutes**

| Time | Activity |
|------|----------|
| 10 min | Review health trends |
| 15 min | What helped us stay healthy? |
| 15 min | What hurt our health? |
| 15 min | What should we change? |
| 5 min | Commit to 2-3 actions |

## Framework: 1:1 Health Check Questions

Regular questions for managers:

| Question | What It Reveals |
|----------|-----------------|
| "How sustainable does your workload feel?" | Capacity |
| "What's the most frustrating part of your job right now?" | Pain points |
| "Do you have everything you need to do your best work?" | Blockers |
| "When did you last take a real day off?" | Rest |
| "What would make next week better than this one?" | Actionable improvement |
| "Is there anything I should know that you haven't told me?" | Hidden issues |

## Checklist

- [ ] Pulse survey implemented
- [ ] Frequency decided
- [ ] Health dashboard created
- [ ] Warning signs documented
- [ ] Response protocol defined
- [ ] Sustainable pace guidelines set
- [ ] Manager check-in questions provided
- [ ] Quarterly health retro scheduled

## Tasks

1. **Implement pulse survey** with chosen tool
2. **Baseline your team health** with first survey
3. **Create health dashboard** to track trends
4. **Define your sustainable pace** guidelines
5. **Train managers** on health conversations

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# Track A Summary

## Team Structure Checklist

Before proceeding to Block 4 (Daily Production & Execution), confirm:

| Team Structure Element | Complete? | Location |
|-----------------------|-----------|----------|
| RACI Matrix | | |
| Decision Rights | | |
| Handoff Protocols | | |
| Meeting Taxonomy | | |
| War Room Protocol | | |
| Stand-up Format | | |
| Async Standards | | |
| Data Sharing Process | | |
| Vendor Management | | |
| On-Call Rotation | | |
| Feedback Loop | | |
| Onboarding Checklist | | |
| Knowledge Base | | |
| Conflict Resolution | | |
| Team Health Pulse | | |

## Red Flags to Address

- [ ] RACI has multiple "A"s per decision
- [ ] Decision rights unclear—frequent escalations
- [ ] Handoffs causing delays or quality issues
- [ ] Meetings consuming >40% of time
- [ ] No on-call coverage for live operations
- [ ] Feedback not reaching product decisions
- [ ] New hires taking >1 month to be productive
- [ ] Team health scores declining
- [ ] Conflict avoided rather than resolved
