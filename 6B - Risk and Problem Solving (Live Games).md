---
layout: default
title: "Risk and Problem Solving (Live Games)"
---

# Risk & Problem Solving (Live Games)

Complete this track to strengthen operational resilience. Return when incidents increase, response times suffer, or team health declines.

---

# 6B.1 Risk Register — Live Ops

## Why It Matters

Live games face different risks than development projects. Server outages, economy exploits, negative review spikes, content bugs, and event failures can destroy months of goodwill in hours. A live ops risk register tracks operational risks that threaten the running game—risks that require different response mechanisms than development risks.

## Framework: Live Ops Risk Categories

```
┌─────────────────────────────────────────────────────────────────────┐
│                    LIVE OPS RISK CATEGORIES                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  🖥️ INFRASTRUCTURE                                                  │
│  ├── Server outages and degradation                                 │
│  ├── Database failures and data loss                                │
│  ├── CDN and content delivery issues                                │
│  ├── Third-party service outages (auth, payments, analytics)        │
│  └── Platform service disruptions                                   │
│                                                                     │
│  💰 ECONOMY                                                         │
│  ├── Duplication exploits                                           │
│  ├── Currency/resource generation bugs                              │
│  ├── Unintended discounts or free purchases                         │
│  ├── Economy inflation/deflation spirals                            │
│  └── Black market/RMT disruption                                    │
│                                                                     │
│  🎮 CONTENT                                                         │
│  ├── Events failing to start/end correctly                          │
│  ├── Broken or unfair game mechanics                                │
│  ├── Missing or wrong rewards                                       │
│  ├── Localization errors                                            │
│  └── Content not appearing for segments                             │
│                                                                     │
│  📉 SENTIMENT                                                       │
│  ├── Negative review spikes                                         │
│  ├── Social media backlash                                          │
│  ├── Community revolt (Discord, Reddit, forums)                     │
│  ├── Influencer criticism                                           │
│  └── Press coverage of issues                                       │
│                                                                     │
│  🔒 SECURITY                                                        │
│  ├── Account compromises                                            │
│  ├── Cheating and botting                                           │
│  ├── DDoS attacks                                                   │
│  └── Data breaches                                                  │
│                                                                     │
│  📊 DATA                                                            │
│  ├── Analytics pipeline failures                                    │
│  ├── A/B test contamination                                         │
│  ├── Reporting inaccuracies                                         │
│  └── Attribution issues                                             │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Live Ops Risk Register Template

| ID | Risk | Category | Likelihood | Impact | Score | Detection | Response Plan | Owner |
|----|------|----------|------------|--------|-------|-----------|---------------|-------|
| LR001 | | | 1-5 | 1-5 | L×I | How we'd know | What we'd do | |
| LR002 | | | | | | | | |
| LR003 | | | | | | | | |
| LR004 | | | | | | | | |
| LR005 | | | | | | | | |

## Framework: Live Ops Impact Scale

| Score | Revenue Impact | User Impact | Duration | Example |
|-------|---------------|-------------|----------|---------|
| 1 | <$1K | <100 users | <1 hour | Minor config error, quick fix |
| 2 | $1K-$10K | 100-1K users | 1-4 hours | Event reward wrong, corrected quickly |
| 3 | $10K-$50K | 1K-10K users | 4-24 hours | Feature broken for a day |
| 4 | $50K-$250K | 10K-100K users | 1-7 days | Major event failure, compensation needed |
| 5 | >$250K | 100K+ users | 7+ days | Server outage, major exploit, review bomb |

*Adjust thresholds to your game's scale*

## Framework: Common Live Ops Risks

| Risk | Likelihood | Typical Impact | Detection Method | Response Time Target |
|------|------------|----------------|------------------|---------------------|
| **Server outage** | Medium | Critical | Monitoring alerts | <15 min detection, <1 hr resolution |
| **Economy exploit** | Medium | High-Critical | Player reports, anomaly detection | <4 hrs detection, same day response |
| **Event misconfiguration** | High | Medium-High | QA, player reports | <1 hr detection, <2 hr fix |
| **Negative review spike** | Medium | Medium | Review monitoring | <24 hr detection, same day response |
| **Payment issues** | Low | High | Support tickets, monitoring | <1 hr detection, immediate escalation |
| **Cheating wave** | Medium | Medium-High | Reports, data analysis | Days to detect, weeks to address |

## Framework: Your Live Ops Risk Audit

Review recent history to calibrate your register:

| Time Period | Incidents | Most Severe | Root Cause | Prevented Now? |
|-------------|-----------|-------------|------------|----------------|
| Last 30 days | | | | |
| Last 90 days | | | | |
| Last year | | | | |

**Patterns identified:** _______________

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| When was the last major live incident? | | Recency of pain |
| What's our average incident response time? | | Response capability |
| Which risk category has most incidents? | | Focus area |
| Do we have monitoring for all critical risks? | | Detection gaps |
| Are response plans documented and tested? | | Readiness |

## Checklist

- [ ] All risk categories assessed
- [ ] Top 10-15 live ops risks documented
- [ ] Likelihood and impact scored
- [ ] Detection methods identified for each
- [ ] Response plans documented
- [ ] Owners assigned
- [ ] Review cadence established

## Tasks

1. **Audit last year's incidents** — what actually happened?
2. **Identify detection gaps** — what could happen unnoticed?
3. **Document response plans** for top 5 risks
4. **Assign owners** — who responds to each category?
5. **Test a response plan** — tabletop exercise

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.2 Operational Risk Prioritization

## Why It Matters

Live ops teams can't prepare equally for every possible problem. Prioritization focuses limited preparation time on risks that are most likely and most damaging. This differs from development risk prioritization because live ops risks often require immediate response playbooks, not just mitigation plans.

## Framework: Live Ops Risk Matrix

```
                              IMPACT (Revenue + User + Reputation)
                 1          2          3          4          5
              Minimal    Minor    Moderate    Major    Critical
           ┌──────────┬──────────┬──────────┬──────────┬──────────┐
         5 │ MONITOR  │ PLAYBOOK │ PLAYBOOK │ WAR ROOM │ WAR ROOM │
   Almost  │          │ READY    │ + DRILL  │ + DRILL  │ + DRILL  │
   Certain │          │          │          │          │ + BACKUP │
           ├──────────┼──────────┼──────────┼──────────┼──────────┤
         4 │ MONITOR  │ MONITOR  │ PLAYBOOK │ PLAYBOOK │ WAR ROOM │
   Likely  │          │          │ READY    │ + DRILL  │ + DRILL  │
           │          │          │          │          │          │
L          ├──────────┼──────────┼──────────┼──────────┼──────────┤
I        3 │ ACCEPT   │ MONITOR  │ MONITOR  │ PLAYBOOK │ PLAYBOOK │
K Possible │          │          │          │ READY    │ + DRILL  │
E          │          │          │          │          │          │
L          ├──────────┼──────────┼──────────┼──────────┼──────────┤
I        2 │ ACCEPT   │ ACCEPT   │ MONITOR  │ MONITOR  │ PLAYBOOK │
H Unlikely │          │          │          │          │ READY    │
O          │          │          │          │          │          │
O          ├──────────┼──────────┼──────────┼──────────┼──────────┤
D        1 │ ACCEPT   │ ACCEPT   │ ACCEPT   │ MONITOR  │ MONITOR  │
     Rare  │          │          │          │          │          │
           │          │          │          │          │          │
           └──────────┴──────────┴──────────┴──────────┴──────────┘
```

## Framework: Response Readiness Levels

| Level | Description | Investment Required |
|-------|-------------|---------------------|
| **ACCEPT** | Acknowledge risk, no specific preparation | None—handle ad hoc if occurs |
| **MONITOR** | Have detection in place | Monitoring setup, alerts configured |
| **PLAYBOOK READY** | Documented response procedure | Response playbook written, owners identified |
| **PLAYBOOK + DRILL** | Tested response procedure | Regular drills, playbook validated |
| **WAR ROOM + DRILL** | Full incident response capability | War room protocol, communication plan, tested |
| **WAR ROOM + BACKUP** | Full redundancy | Backup systems, automated failover, tested recovery |

## Framework: Risk Investment Prioritization

| Risk | Score | Current Readiness | Target Readiness | Gap | Priority |
|------|-------|-------------------|------------------|-----|----------|
| | | Accept/Monitor/Playbook/Drill/War Room | | | 1-10 |
| | | | | | |
| | | | | | |
| | | | | | |
| | | | | | |

## Framework: Detection Investment Checklist

| Risk | Current Detection | Detection Gap | Investment to Close |
|------|-------------------|---------------|---------------------|
| Server outage | | ☐ None ☐ Partial ☐ Complete | |
| Economy exploit | | ☐ None ☐ Partial ☐ Complete | |
| Event failure | | ☐ None ☐ Partial ☐ Complete | |
| Review spike | | ☐ None ☐ Partial ☐ Complete | |
| Payment issues | | ☐ None ☐ Partial ☐ Complete | |
| Cheating | | ☐ None ☐ Partial ☐ Complete | |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| Which high-impact risks lack playbooks? | | Preparation gap |
| When did we last drill a response? | | Rust on procedures |
| What's our detection coverage? | | Blind spots |
| Are playbooks current and accessible? | | Documentation debt |
| Do new team members know response protocols? | | Knowledge transfer |

## Checklist

- [ ] All high-scoring risks have appropriate readiness level
- [ ] Detection mechanisms in place for monitor+ risks
- [ ] Playbooks documented for playbook+ risks
- [ ] Drills scheduled for drill+ risks
- [ ] War room protocol defined for war room+ risks
- [ ] Investment plan for closing gaps

## Tasks

1. **Plot all live ops risks** on the matrix
2. **Assess current readiness** for each
3. **Identify gaps** between current and target
4. **Prioritize investments** based on gaps
5. **Schedule drills** for top risks

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.3 Economy Exploit Response Plan

## Why It Matters

Economy exploits are among the most damaging live ops incidents. A duplication bug or currency generation exploit can destroy months of careful balancing in hours. Worse, how you respond affects player trust as much as the exploit itself. A clear response plan enables fast, fair, consistent action when seconds count.

## Framework: Exploit Response Phases

```
┌─────────────────────────────────────────────────────────────────────┐
│                    ECONOMY EXPLOIT RESPONSE                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  PHASE 1: DETECT (Minutes)                                          │
│  ├── Automated anomaly alerts                                       │
│  ├── Player reports                                                 │
│  ├── Community chatter                                              │
│  └── Internal discovery                                             │
│                           │                                          │
│                           ▼                                          │
│  PHASE 2: ASSESS (< 1 Hour)                                         │
│  ├── Confirm exploit is real                                        │
│  ├── Determine scope (how many affected, how much gained)           │
│  ├── Identify exploit mechanism                                     │
│  ├── Assess if still exploitable                                    │
│  └── Estimate total damage                                          │
│                           │                                          │
│                           ▼                                          │
│  PHASE 3: CONTAIN (< 4 Hours)                                       │
│  ├── Stop the bleeding (disable feature, take server down, hotfix)  │
│  ├── Communicate to players (if visible)                            │
│  └── Preserve evidence                                              │
│                           │                                          │
│                           ▼                                          │
│  PHASE 4: REMEDIATE (Hours to Days)                                 │
│  ├── Decide: rollback vs. compensation vs. let it stand            │
│  ├── Identify exploiters (if acting against)                        │
│  ├── Execute remedy                                                 │
│  ├── Communicate decisions                                          │
│  └── Fix root cause                                                 │
│                           │                                          │
│                           ▼                                          │
│  PHASE 5: LEARN (Days)                                              │
│  ├── Post-mortem                                                    │
│  ├── Process improvements                                           │
│  └── Detection improvements                                         │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Exploit Severity Classification

| Severity | Definition | Response Target | Example |
|----------|------------|-----------------|---------|
| **Critical** | Game-breaking, spreading rapidly, massive economy impact | Contain in <1 hour | Infinite currency generation |
| **High** | Significant advantage, many exploiters | Contain in <4 hours | Duplication bug |
| **Medium** | Moderate advantage, limited spread | Contain in <24 hours | Event reward exploit |
| **Low** | Minor advantage, few exploiters | Next update | Minor pricing error |

## Framework: Remediation Decision Matrix

| Factor | Rollback | Negative Adjustment | Let Stand | Compensation |
|--------|----------|---------------------|-----------|--------------|
| **Exploiters only** | Complex to target | Easiest if identifiable | Unfair to non-exploiters | Doesn't help |
| **Widespread (>10% players)** | High impact | Causes outrage | Consider if minimal damage | Expensive |
| **Time since exploit** | <24 hrs: possible | Anytime | More palatable later | Anytime |
| **Damage severity** | High: consider | High: necessary | Low: often OK | High: consider |
| **Player intent** | Clear abuse: act | Clear abuse: act | Accidental: forgive | All affected |

## Framework: Decision Flowchart

```
                    Exploit Confirmed
                          │
                          ▼
                  Is it still active?
                   ┌──────┴──────┐
                   │             │
                  YES           NO
                   │             │
                   ▼             │
              Contain first      │
                   │             │
                   └──────┬──────┘
                          │
                          ▼
                  How severe is damage?
           ┌──────────────┼──────────────┐
           │              │              │
        CRITICAL      MODERATE         LOW
           │              │              │
           ▼              ▼              ▼
    Consider rollback  Target    Let stand or
    or server action   exploiters    note only
           │              │              │
           └──────────────┼──────────────┘
                          │
                          ▼
                  Communicate decision
                          │
                          ▼
                  Execute & document
```

## Framework: Communication Templates

### Initial Acknowledgment (Within 1 hour of containment)

```
We're aware of an issue affecting [affected area]. We've taken 
[containment action] while we investigate. We'll share more 
information soon. Thank you for your patience.
```

### Decision Communication

```
UPDATE on [issue]:

WHAT HAPPENED: [Brief factual description]

WHAT WE'RE DOING: [Specific actions]
- [Action 1]
- [Action 2]

TIMELINE: [When players can expect resolution]

We apologize for any inconvenience and appreciate your understanding.
```

### Compensation Announcement

```
To make up for [issue], all players [affected players] will receive:
- [Compensation item 1]
- [Compensation item 2]

This will be delivered to your inbox by [time/date].

We've also [specific fix] to prevent this from happening again.
```

## Framework: Exploit Response Checklist

### Detection Phase
- [ ] Alert received or report confirmed
- [ ] Initial assessment: real exploit?
- [ ] Severity classified
- [ ] Response team notified

### Assessment Phase
- [ ] Exploit mechanism understood
- [ ] Scope quantified (users, currency, items)
- [ ] Still exploitable?
- [ ] Evidence preserved (logs, screenshots)

### Containment Phase
- [ ] Exploit stopped (feature disabled, server action, hotfix)
- [ ] Players notified if visible
- [ ] Escalation to leadership if high severity

### Remediation Phase
- [ ] Decision made: rollback / adjust / let stand / compensate
- [ ] Exploiter list generated (if acting)
- [ ] Remedy executed
- [ ] Communication sent

### Learning Phase
- [ ] Post-mortem scheduled
- [ ] Root cause documented
- [ ] Prevention measures identified

## Framework: Your Response Team

| Role | Responsibility | Primary | Backup |
|------|----------------|---------|--------|
| **Incident Commander** | Coordinates response, makes decisions | | |
| **Technical Lead** | Diagnoses exploit, implements fix | | |
| **Data Analyst** | Quantifies damage, identifies exploiters | | |
| **Community Manager** | Player communication | | |
| **Producer** | Stakeholder communication, authorization | | |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| When was our last economy exploit? | | Recency of experience |
| How quickly did we detect it? | | Detection capability |
| How quickly did we contain it? | | Response capability |
| Did our response feel fair to players? | | Communication quality |
| Did we prevent recurrence? | | Learning effectiveness |

## Checklist

- [ ] Response phases understood by team
- [ ] Severity classification defined
- [ ] Remediation decision framework agreed
- [ ] Communication templates prepared
- [ ] Response checklist accessible
- [ ] Response team identified with backups
- [ ] Detection mechanisms in place
- [ ] Post-mortem process defined

## Tasks

1. **Review past exploits** — how did we respond?
2. **Define severity thresholds** for your economy
3. **Prepare communication templates**
4. **Assign response team roles**
5. **Tabletop exercise** — walk through a scenario
6. **Improve detection** — can you catch exploits faster?

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.4 Server Incident Protocol

## Why It Matters

Server outages are the most visible form of live ops failure. Every minute of downtime is lost revenue, frustrated players, and negative reviews. A clear incident protocol reduces chaos, accelerates recovery, and ensures communication happens appropriately. The middle of an outage is not the time to figure out who does what.

## Framework: Incident Severity Levels

| Severity | Definition | Response | Communication | Examples |
|----------|------------|----------|---------------|----------|
| **SEV 1** | Complete outage, all users affected | All-hands war room | Immediate public acknowledgment | Server down, database corruption |
| **SEV 2** | Major degradation, many users affected | Core team response | Public acknowledgment within 1 hour | Severe lag, payment failures |
| **SEV 3** | Partial degradation, some users affected | On-call response | Update status page | Feature broken, regional issues |
| **SEV 4** | Minor issue, minimal user impact | Normal priority | No public communication | Cosmetic bugs, minor errors |

## Framework: War Room Activation

```
┌─────────────────────────────────────────────────────────────────────┐
│                    WAR ROOM PROTOCOL                                 │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  TRIGGER: SEV 1 or SEV 2 incident confirmed                         │
│                                                                     │
│  WITHIN 5 MINUTES:                                                  │
│  ├── War room channel created (Slack/Discord/Bridge)                │
│  ├── Incident Commander identified                                  │
│  ├── On-call engineers joined                                       │
│  └── Initial status update posted                                   │
│                                                                     │
│  WITHIN 15 MINUTES:                                                 │
│  ├── Scope of impact assessed                                       │
│  ├── Initial hypothesis formed                                      │
│  ├── External communication drafted                                 │
│  └── Leadership notified                                            │
│                                                                     │
│  ONGOING:                                                           │
│  ├── 15-minute status updates in war room                           │
│  ├── External updates every 30 minutes                              │
│  ├── Decisions logged                                               │
│  └── Relief scheduled if extended (>4 hours)                        │
│                                                                     │
│  RESOLUTION:                                                        │
│  ├── Recovery confirmed via monitoring                              │
│  ├── Final external communication sent                              │
│  ├── War room closed                                                │
│  └── Post-mortem scheduled                                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Incident Response Roles

| Role | Responsibility | Who | Backup |
|------|----------------|-----|--------|
| **Incident Commander (IC)** | Coordinates response, makes decisions, manages communication | | |
| **Technical Lead** | Leads diagnosis and fix, directs engineering effort | | |
| **Communications Lead** | Drafts and sends player-facing messages | | |
| **Scribe** | Documents timeline, decisions, actions in real-time | | |
| **Subject Matter Expert** | Provides expertise on affected systems | Varies | |

### Incident Commander Responsibilities

- Declares incident severity
- Opens war room
- Assigns roles
- Coordinates workstreams
- Makes escalation decisions
- Approves communications
- Declares resolution
- Triggers post-mortem

## Framework: Communication Protocol

| Timing | Audience | Content | Channel |
|--------|----------|---------|---------|
| **0 min** | Internal | Incident declared, war room open | Slack/Teams |
| **5-15 min** | Players | Acknowledgment: "We're aware and investigating" | Status page, social |
| **Every 30 min** | Players | Status update with ETA if known | Status page, social |
| **Resolution** | Players | "Resolved" with brief explanation | Status page, social |
| **Follow-up** | Players | Post-mortem summary, compensation if applicable | Blog, in-game |

### Communication Templates

**Initial Acknowledgment:**
```
⚠️ We're experiencing issues affecting [game/service]. Our team is 
investigating. We'll update every 30 minutes. Thank you for your patience.
```

**Status Update:**
```
🔄 UPDATE: We've identified the issue as [brief description]. We're 
working on a fix. Estimated resolution: [time] or "unknown at this time."
```

**Resolution:**
```
✅ RESOLVED: [Game/Service] is now operating normally. The issue was 
caused by [brief cause]. We apologize for the inconvenience. [Compensation 
details if applicable]
```

## Framework: Incident Timeline Log Template

| Time | Event | Actions | Decisions | By |
|------|-------|---------|-----------|-----|
| | Incident detected | | | |
| | War room opened | | | |
| | | | | |
| | | | | |
| | Incident resolved | | | |
| | War room closed | | | |

## Framework: Post-Incident Checklist

- [ ] Recovery confirmed via monitoring
- [ ] Final player communication sent
- [ ] War room archived (not deleted)
- [ ] Timeline documented
- [ ] Impact quantified (users, duration, revenue)
- [ ] Post-mortem scheduled (within 48 hours)
- [ ] Compensation decision made
- [ ] Stakeholders debriefed

## Framework: On-Call Structure

| Coverage | Hours | Primary | Secondary |
|----------|-------|---------|-----------|
| Business hours | | | |
| Evening | | | |
| Weekend | | | |
| Holiday | | | |

### On-Call Responsibilities

- Respond to pages within [X] minutes
- Assess severity and escalate if needed
- Begin triage and diagnosis
- Open war room if SEV 1/2
- Stay engaged until handed off or resolved

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What's our average incident response time? | | Response speed |
| What's our average time to resolution? | | Recovery capability |
| How often do we have SEV 1 incidents? | | System reliability |
| Is on-call coverage sustainable? | | Team health |
| Do we post-mortem every incident? | | Learning culture |

## Checklist

- [ ] Severity levels defined and calibrated
- [ ] War room protocol documented
- [ ] Response roles assigned with backups
- [ ] Communication protocol established
- [ ] Templates prepared
- [ ] On-call rotation in place
- [ ] Escalation paths clear
- [ ] Post-incident process defined

## Tasks

1. **Define your severity levels** with specific examples
2. **Assign incident roles** with backups
3. **Create communication templates**
4. **Set up war room infrastructure** (channel, bridge)
5. **Establish on-call rotation**
6. **Run a drill** — practice with a simulated incident

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.5 Negative Review Spike Response

## Why It Matters

In mobile and PC gaming, ratings directly affect store visibility and conversion. A negative review spike can trigger a death spiral: bad ratings → less visibility → fewer installs → less revenue → less development → worse game → worse ratings. Rapid detection and response can stop this spiral before it becomes irreversible.

## Framework: Review Health Monitoring

```
┌─────────────────────────────────────────────────────────────────────┐
│                    REVIEW MONITORING DASHBOARD                       │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  KEY METRICS TO TRACK                                               │
│  ├── Overall rating (rolling average)                               │
│  ├── Rating by version (is new version causing drop?)               │
│  ├── Daily review volume (spike = something happened)               │
│  ├── Sentiment distribution (1★ vs 5★ ratio)                        │
│  ├── Rating by platform/region (localized issues)                   │
│  └── Review text themes (what are people saying?)                   │
│                                                                     │
│  ALERT THRESHOLDS                                                   │
│  ├── Rating drops >0.1 in 24 hours                                  │
│  ├── 1★ reviews double normal rate                                  │
│  ├── Specific terms spiking (bug, crash, broken, scam)              │
│  └── Rating below [your threshold] for [time period]                │
│                                                                     │
│  MONITORING CADENCE                                                 │
│  ├── Automated: Continuous with alerts                              │
│  ├── Manual check: Daily                                            │
│  └── Deep analysis: Weekly or after releases                        │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Root Cause Categories

| Category | Common Triggers | Typical Velocity | Recovery Approach |
|----------|-----------------|------------------|-------------------|
| **Bug/Crash** | New update, server issues | Fast spike | Fix bug, communicate, request re-review |
| **Balance/Fairness** | Economy change, P2W perception | Medium spike | Adjust or explain reasoning |
| **Missing feature** | Feature removal, expected feature absent | Medium spike | Communicate roadmap or restore |
| **Monetization** | Price increase, aggressive IAP | Medium spike | Adjust strategy or messaging |
| **Performance** | Device issues, battery, heating | Slow build | Optimization update |
| **External event** | Competitor launch, controversy, news | Can vary | Community engagement |

## Framework: Response Decision Matrix

| Situation | Response Speed | Actions |
|-----------|----------------|---------|
| **Clear bug causing reviews** | Immediate | Fix → Hotfix → Request re-reviews |
| **Controversial change, mixed response** | 24-48 hours | Analyze data, communicate reasoning, consider adjustment |
| **Perception issue (game unchanged)** | 48-72 hours | Communication campaign, surface positive aspects |
| **Competitive/external factors** | Ongoing | Focus on product improvement, long-term positioning |

## Framework: Review Spike Response Checklist

### Detection Phase
- [ ] Spike detected (automated or manual)
- [ ] Severity assessed (magnitude, velocity)
- [ ] Initial root cause hypothesized
- [ ] Relevant team notified

### Analysis Phase
- [ ] Reviews read and categorized (sample of 50+)
- [ ] Themes identified and quantified
- [ ] Root cause confirmed or refined
- [ ] Impact on KPIs assessed (installs, conversion)

### Response Phase
- [ ] Fix identified (if technical issue)
- [ ] Communication drafted
- [ ] Response strategy chosen
- [ ] Stakeholders aligned

### Recovery Phase
- [ ] Fix deployed (if applicable)
- [ ] Communication sent
- [ ] Re-review requests initiated (if appropriate)
- [ ] Ratings monitored for recovery
- [ ] Learnings documented

## Framework: Communication Approaches

| Approach | When to Use | Example |
|----------|-------------|---------|
| **Acknowledge + Fix coming** | Clear bug, fix in progress | "We're aware of crashes and a fix is coming tomorrow" |
| **Explain reasoning** | Controversial intentional change | "Here's why we made this change and what we heard" |
| **Gather feedback** | Unclear root cause | "Help us understand what's not working" |
| **Highlight improvements** | Perception lag vs. reality | "In recent updates, we've improved..." |
| **Silence** | External factors, will pass | Monitor but don't amplify |

### Response Channels

| Channel | Speed | Reach | Best For |
|---------|-------|-------|----------|
| **In-app message** | Immediate | All active users | Widespread issues |
| **Store description** | Hours | Potential installs | Known issues, incoming fixes |
| **Social media** | Immediate | Followers | Quick acknowledgment |
| **Community (Discord/Reddit)** | Immediate | Engaged players | Detailed discussion |
| **Email** | Hours | Subscribed users | Important announcements |
| **Review response** | Hours | Individual reviewer | Direct engagement |

## Framework: Re-Review Request Strategy

When and how to ask players to update their reviews:

| Timing | Method | Effectiveness |
|--------|--------|---------------|
| **After fix deployed** | In-app prompt to affected users | High if fix resolves issue |
| **After positive experience** | After level completion, purchase, win | Medium, generic |
| **Direct response to review** | Reply to negative review with fix | Medium, shows engagement |

**Do:**
- Target users who experienced the fixed issue
- Time request after positive moment
- Make it easy (one tap to store)
- Thank them for feedback

**Don't:**
- Spam all users
- Request before fixing the issue
- Offer incentives (violates store policies)
- Be defensive in responses

## Framework: Rating Recovery Plan Template

| Week | Target | Actions | Success Metric |
|------|--------|---------|----------------|
| 1 | Stop bleeding | Fix immediate issues, communicate | Review velocity normalizes |
| 2 | Stabilize | Address secondary complaints, quality updates | Rating stops declining |
| 3-4 | Recover | Push positive content, re-review requests | Rating starts climbing |
| 5+ | Sustain | Maintain quality, regular updates | Rating at/above target |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What's our current rating vs. 3 months ago? | | Trend direction |
| What % of reviews are 1★? | | Severity of issues |
| What themes appear in recent 1★ reviews? | | Root cause hints |
| How quickly do we detect review spikes? | | Monitoring effectiveness |
| When did we last respond publicly to reviews? | | Engagement level |

## Checklist

- [ ] Review monitoring in place
- [ ] Alert thresholds configured
- [ ] Root cause categories understood
- [ ] Response decision matrix adopted
- [ ] Communication templates prepared
- [ ] Re-review request strategy defined
- [ ] Recovery plan template ready
- [ ] Team knows escalation path

## Tasks

1. **Set up monitoring** — automated alerts for rating drops
2. **Baseline your metrics** — know what "normal" looks like
3. **Read 100 recent reviews** — understand current sentiment
4. **Prepare response templates** for common scenarios
5. **Define escalation** — when does leadership need to know?
6. **Create recovery plan** if currently below target

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.6 Rollback Protocol

## Why It Matters

Not every release goes well. When a new feature breaks things, when a config change causes problems, when an event doesn't work as intended—you need to be able to undo. A clear rollback protocol means faster recovery, less arguing about what to do, and confidence to release knowing you have a safety net.

## Framework: Rollback Types

```
┌─────────────────────────────────────────────────────────────────────┐
│                    ROLLBACK TYPES                                    │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ⚙️ CONFIG ROLLBACK (Minutes)                                       │
│  ├── Remote config values                                           │
│  ├── Feature flags                                                  │
│  ├── Event settings                                                 │
│  ├── Economy values                                                 │
│  └── A/B test assignments                                           │
│                                                                     │
│  🔄 SERVER ROLLBACK (Minutes to Hours)                              │
│  ├── Backend deployment                                             │
│  ├── API version                                                    │
│  ├── Database migration (complex)                                   │
│  └── Infrastructure changes                                         │
│                                                                     │
│  📱 CLIENT ROLLBACK (Days to Weeks)                                 │
│  ├── App store version (requires review)                            │
│  ├── Asset bundles (if supported)                                   │
│  └── Forced update rollback (emergency only)                        │
│                                                                     │
│  💰 ECONOMY ROLLBACK (Hours to Days)                                │
│  ├── Player currency adjustments                                    │
│  ├── Item grants/removals                                           │
│  ├── Purchase reversals                                             │
│  └── Progress resets                                                │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Rollback Decision Matrix

| Scenario | Rollback Type | Decision Time | Decision Maker | Recovery Time |
|----------|---------------|---------------|----------------|---------------|
| Feature flag causes crashes | Config | <15 min | On-call engineer | Minutes |
| Event rewards wrong | Config | <30 min | Live ops + producer | Minutes |
| Server deployment breaks API | Server | <1 hour | Engineering lead | Minutes-hours |
| Client update has major bug | Client | <24 hours | Product lead | Days (store review) |
| Economy exploit discovered | Economy | <4 hours | Producer + director | Hours-days |

## Framework: Rollback Prerequisites

What you need in place BEFORE you can roll back:

| Rollback Type | Prerequisites | Current Status |
|---------------|---------------|----------------|
| **Config** | ☐ Previous values documented ☐ Remote config system ☐ Rollback tested | |
| **Server** | ☐ Previous deployment tagged ☐ Blue-green or staged deployment ☐ Rollback procedure documented | |
| **Client** | ☐ Previous build available ☐ Expedited review relationship ☐ Forced update capability | |
| **Economy** | ☐ Transaction logs complete ☐ Bulk adjustment tools ☐ Audit trail | |

## Framework: Rollback Checklist

### Config Rollback

- [ ] Issue confirmed and severity assessed
- [ ] Decision maker approves rollback
- [ ] Previous config values identified
- [ ] Rollback executed
- [ ] Verification: issue resolved
- [ ] Player communication (if visible)
- [ ] Root cause documented
- [ ] Post-mortem scheduled if high severity

### Server Rollback

- [ ] Issue confirmed and severity assessed
- [ ] Rollback decision approved by engineering lead
- [ ] Previous deployment version identified
- [ ] Traffic shift or blue-green flip executed
- [ ] Verification: monitoring confirms recovery
- [ ] Player communication if there was visible impact
- [ ] Forward fix planned (can't stay on old version forever)
- [ ] Post-mortem scheduled

### Client Rollback

- [ ] Severity justifies emergency measures
- [ ] Director/VP approval obtained
- [ ] Platform contacted for expedited review (if needed)
- [ ] Previous build prepared and submitted
- [ ] Communication plan for players
- [ ] Forced update decision made (if applicable)
- [ ] Timeline communicated internally
- [ ] Post-mortem scheduled

### Economy Rollback

- [ ] Exploit/issue confirmed
- [ ] Scope quantified (players, currency/items, time window)
- [ ] Rollback approach decided (see Economy Exploit Response Plan)
- [ ] Affected players identified
- [ ] Adjustments executed
- [ ] Verification: economy normalized
- [ ] Communication sent to affected players
- [ ] Post-mortem scheduled

## Framework: Rollback Communication Templates

**For visible issues (players noticed):**
```
We've identified an issue with [feature/content] and have reverted to 
the previous version while we investigate. You may notice [expected 
player impact]. We apologize for the inconvenience and will have a 
fix ready soon.
```

**For invisible rollbacks (players didn't notice):**
No communication needed—just fix and move on.

**For economy adjustments:**
```
We discovered an issue that affected [currency/items] for some players. 
To ensure fairness, we've [action taken]. If you believe you were 
affected incorrectly, please contact support.
```

## Framework: Rollback Risk Assessment

Before each release, assess rollback risk:

| Release Component | Rollback Difficulty | Risk if Rollback Needed | Rollback Plan |
|-------------------|---------------------|------------------------|---------------|
| | Easy/Medium/Hard/Impossible | Low/Medium/High | |
| | | | |
| | | | |

### High-Risk Release Preparation

If rollback would be difficult or impossible:

- [ ] Extended testing before release
- [ ] Staged rollout (% of users)
- [ ] Real-time monitoring during rollout
- [ ] Kill switch / feature flag in place
- [ ] Communication plan if issues arise
- [ ] Decision criteria for stopping rollout

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| When did we last roll back? | | Recency of experience |
| How long did it take? | | Execution speed |
| Did we have the right tools? | | Capability gaps |
| Was the decision process clear? | | Process clarity |
| Could we roll back our current release? | | Current readiness |

## Checklist

- [ ] Rollback types documented for your systems
- [ ] Prerequisites in place for each type
- [ ] Checklists accessible to response team
- [ ] Decision makers identified
- [ ] Communication templates prepared
- [ ] Rollback tested in staging
- [ ] Release risk assessment process defined

## Tasks

1. **Inventory your rollback capabilities** — what can you actually undo?
2. **Identify gaps** — what can't you roll back easily?
3. **Invest in critical gaps** — especially config and server
4. **Document procedures** — step-by-step for each type
5. **Test a rollback** — in staging or during low-risk release
6. **Add to release checklist** — rollback plan required before release

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.7 Burnout Early Warning System

## Why It Matters

Live games never stop. There's always another event, another incident, another deadline. This "always-on" nature creates chronic stress that can lead to burnout—especially for teams without structural protections. Burnout causes turnover, reduces quality, and creates institutional knowledge loss. An early warning system catches problems before they become crises.

## Framework: Burnout Indicators

```
┌─────────────────────────────────────────────────────────────────────┐
│                    BURNOUT WARNING SIGNS                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  📊 QUANTITATIVE SIGNALS                                            │
│  ├── Sustained overtime (>45 hrs/week for 3+ weeks)                 │
│  ├── PTO not being taken                                            │
│  ├── Sick days increasing                                           │
│  ├── On-call rotations skewing (same people always responding)      │
│  ├── Incident response times increasing                             │
│  └── Velocity declining despite same hours                          │
│                                                                     │
│  🗣️ QUALITATIVE SIGNALS                                             │
│  ├── Cynicism in team discussions                                   │
│  ├── Reduced participation in planning/retros                       │
│  ├── Increased conflict or short tempers                            │
│  ├── Withdrawal from social interaction                             │
│  ├── Complaints about workload becoming chronic                     │
│  └── "I don't care anymore" statements                              │
│                                                                     │
│  🚪 LEADING INDICATORS                                              │
│  ├── Talking about other opportunities                              │
│  ├── Disengagement from long-term planning                          │
│  ├── Reduced quality standards ("good enough")                      │
│  ├── Avoiding new responsibilities                                  │
│  └── Absenteeism (mental or physical)                               │
│                                                                     │
│  ⚠️ ORGANIZATIONAL PATTERNS                                         │
│  ├── Same people always on-call for incidents                       │
│  ├── No protected time for non-urgent work                          │
│  ├── "Heroes" whose absence would cause crisis                      │
│  ├── Unsustainable content cadence                                  │
│  └── No relief or rotation for high-stress roles                    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Team Health Monitoring

### Weekly Health Check Questions

Ask these in 1:1s or anonymous surveys:

| Question | Scale | Warning Threshold |
|----------|-------|-------------------|
| "How sustainable does your current workload feel?" | 1-5 | <3 for 2+ weeks |
| "Are you able to disconnect from work?" | 1-5 | <3 consistently |
| "Do you feel supported when things get hard?" | 1-5 | <3 |
| "How would you rate your energy level?" | 1-5 | <3 for 2+ weeks |
| "Are you proud of the work you're doing?" | 1-5 | <3 |

### Monthly Metrics Dashboard

| Metric | Target | This Month | Trend | Action if Breached |
|--------|--------|------------|-------|-------------------|
| Avg weekly hours | <45 | | ↑↓→ | Review workload |
| PTO utilization | >80% of accrued | | ↑↓→ | Encourage time off |
| Sick days | Baseline +/-20% | | ↑↓→ | Check on individuals |
| On-call burden | <1 week/month/person | | ↑↓→ | Expand rotation |
| Survey average | >3.5/5 | | ↑↓→ | Deep dive needed |

## Framework: Risk Assessment by Role

| Role | Burnout Risk Factors | Protective Factors | Current Risk |
|------|---------------------|-------------------|--------------|
| **Live Ops Producer** | Always-on, event pressure, incidents | Clear boundaries, backup coverage | |
| **Server Engineer** | On-call, incident stress, late nights | Rotation, comp time | |
| **Community Manager** | Negative feedback, 24/7 social | Clear hours, moderation support | |
| **QA Lead** | End-of-cycle crunch, repetitive work | Automation, schedule padding | |
| **Content Designer** | Cadence pressure, repetition | Template efficiency, creative breaks | |

## Framework: Structural Protections

| Protection | Implementation | Owner | Status |
|------------|----------------|-------|--------|
| **Maximum weekly hours** | Alert at 45, intervention at 50 | Managers | |
| **Mandatory PTO** | Minimum days/quarter, tracked | HR/Managers | |
| **On-call rotation** | Fair distribution, comp time | Engineering lead | |
| **Event buffer** | Padding between event cycles | Live ops lead | |
| **Incident response relief** | Handoff required after 4 hours | IC protocol | |
| **No-meeting recovery time** | Day after major release/incident | Producer | |
| **Protected development time** | % of sprint for non-live work | Producer | |

## Framework: Intervention Levels

| Level | Trigger | Response | Who Acts |
|-------|---------|----------|----------|
| **Watch** | Single warning sign, individual | 1:1 conversation, monitor | Direct manager |
| **Support** | Multiple signs, or pattern | Workload adjustment, resources | Manager + producer |
| **Intervene** | Sustained signals, team pattern | Scope reduction, timeline extension | Director |
| **Escalate** | Team health crisis, attrition risk | Project restructure, leadership review | VP/Exec |

## Framework: Recovery Support

When someone is burned out:

| Phase | Actions | Duration |
|-------|---------|----------|
| **Immediate** | Reduce workload, prioritize ruthlessly, check in daily | 1-2 weeks |
| **Recovery** | Reassign high-stress work, enable time off, light duties | 2-4 weeks |
| **Rebuild** | Gradually increase responsibility, maintain check-ins | 4-8 weeks |
| **Prevent recurrence** | Identify and fix root causes, adjust role if needed | Ongoing |

## Framework: Your Team's Health Profile

| Team Member | Current Hours | PTO Status | On-Call Load | Risk Level | Notes |
|-------------|---------------|------------|--------------|------------|-------|
| | | | | Low/Medium/High | |
| | | | | | |
| | | | | | |
| | | | | | |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What's our average weekly hours over the last month? | | Workload reality |
| Who's had the most on-call incidents? | | Fair distribution |
| When did the team last take significant time off? | | Recovery patterns |
| Have we had any resignations citing workload? | | Retention signal |
| Do managers have regular 1:1s about wellbeing? | | Support structure |

## Checklist

- [ ] Warning signs documented and shared with managers
- [ ] Weekly health check mechanism in place
- [ ] Monthly metrics dashboard maintained
- [ ] Structural protections implemented
- [ ] Intervention levels defined
- [ ] Recovery support process documented
- [ ] Team health profile current
- [ ] Leadership commitment to sustainable pace

## Tasks

1. **Baseline your team health** — survey and hours audit
2. **Implement weekly pulse check** — simple, consistent
3. **Track and review monthly metrics**
4. **Assess structural protections** — what's missing?
5. **Train managers** on warning signs and intervention
6. **Address any current high-risk individuals**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 6B.8 Continuous Improvement & Learning

## Why It Matters

Live games generate constant feedback—from players, from data, from incidents. Teams that learn from this feedback improve. Teams that don't stagnate or regress. A continuous improvement culture makes learning systematic, not accidental. It's the compound interest of operational excellence.

## Framework: Learning Loop Sources

```
┌─────────────────────────────────────────────────────────────────────┐
│                    LEARNING LOOP SOURCES                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  📊 DATA FEEDBACK                                                   │
│  ├── A/B test results                                               │
│  ├── Feature performance metrics                                    │
│  ├── Event post-analysis                                            │
│  ├── Retention/monetization trends                                  │
│  └── Economy health indicators                                      │
│                                                                     │
│  👥 PLAYER FEEDBACK                                                 │
│  ├── Reviews and ratings                                            │
│  ├── Community discussions                                          │
│  ├── Support tickets                                                │
│  ├── Social media sentiment                                         │
│  └── Direct feedback (surveys, interviews)                          │
│                                                                     │
│  🔥 INCIDENT LEARNING                                               │
│  ├── Post-mortems                                                   │
│  ├── Near-miss analysis                                             │
│  ├── Recurring issue patterns                                       │
│  └── Response effectiveness                                         │
│                                                                     │
│  🔄 PROCESS FEEDBACK                                                │
│  ├── Retrospectives                                                 │
│  ├── Efficiency metrics (time to ship, bug rates)                   │
│  ├── Team feedback                                                  │
│  └── Cross-functional friction points                               │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Learning Review Cadence

| Review | Frequency | Scope | Participants | Output |
|--------|-----------|-------|--------------|--------|
| **Sprint retro** | Every sprint | Last sprint | Scrum team | Process improvements |
| **Event retro** | After each event | Single event | Live ops team | Event learnings |
| **Incident post-mortem** | Per significant incident | Single incident | Responders | Prevention actions |
| **Monthly review** | Monthly | Month's operations | Leads | Trend analysis |
| **Quarterly strategy** | Quarterly | Quarter performance | Leadership | Strategic adjustments |

## Framework: Structured Event Retrospective

### Event Performance Review Template

| Dimension | Planned | Actual | Delta | Learning |
|-----------|---------|--------|-------|----------|
| **Participation rate** | | | | |
| **Completion rate** | | | | |
| **Revenue** | | | | |
| **New user conversion** | | | | |
| **Player sentiment** | | | | |
| **Production effort** | | | | |
| **Incidents/issues** | | | | |

### Questions to Ask

- What did players love about this event?
- What frustrated players?
- What surprised us (positive or negative)?
- What would we do differently?
- What should we repeat?
- What should we stop doing?

## Framework: Learning Repository Structure

Maintain a searchable knowledge base:

| Category | Content Types | Example Topics |
|----------|---------------|----------------|
| **Event learnings** | Retros, performance data | "Holiday events perform 30% better with X" |
| **Feature learnings** | A/B results, post-launch data | "Tutorial simplification increased D1 by 5%" |
| **Incident learnings** | Post-mortems | "Always verify config in staging" |
| **Process learnings** | Retro outputs | "Reduced QA time with automated checklist" |
| **Player insights** | Research, feedback analysis | "Players value cosmetics over power" |

## Framework: Action Tracking

| Learning | Source | Action | Owner | Status | Outcome |
|----------|--------|--------|-------|--------|---------|
| | Event/Incident/Retro/Data | | | Open/In Progress/Done | Improved/No change/Worse |
| | | | | | |
| | | | | | |

### Action Quality Criteria

Good actions are:
- **Specific** — Clear what to do
- **Measurable** — Know when it's done
- **Owned** — Single person accountable
- **Timely** — Reasonable deadline
- **Proportionate** — Effort matches learning importance

## Framework: Improvement Metrics

| Metric | Definition | Target | Current | Trend |
|--------|------------|--------|---------|-------|
| **Learning capture rate** | % of events/incidents with documented learnings | >90% | | |
| **Action completion rate** | % of learning actions completed | >75% | | |
| **Time to learn** | Days from event/incident to learning documented | <7 days | | |
| **Recurrence rate** | % of incidents that repeat | <10% | | |
| **Process improvements/quarter** | Number of process changes from learnings | >5 | | |

## Framework: Cross-Team Learning

Learnings shouldn't stay siloed:

| Sharing Mechanism | Frequency | Audience | Format |
|-------------------|-----------|----------|--------|
| **Learning digest** | Weekly | All team | Email/Slack summary |
| **Knowledge base** | Ongoing | All team | Searchable wiki |
| **Monthly deep-dive** | Monthly | Interested team | Presentation + discussion |
| **Onboarding curriculum** | New hire start | New members | Curated reading list |

## Framework: Continuous Improvement Health

### Self-Assessment

| Question | Score (1-5) | Evidence |
|----------|-------------|----------|
| Do we document learnings consistently? | | |
| Do we act on learnings? | | |
| Do learnings prevent repeat problems? | | |
| Is knowledge shared across teams? | | |
| Do we celebrate learning and improvement? | | |

**Total score:** _____ / 25

- 20-25: Strong learning culture
- 15-19: Good foundation, room to improve
- 10-14: Inconsistent, needs investment
- <10: Learning culture absent, priority fix

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What did we learn from our last event? | | Capture consistency |
| When was our last post-mortem? | | Incident learning |
| Can new team members find past learnings? | | Knowledge management |
| What process improved recently because of learnings? | | Action on learnings |
| Do we repeat the same mistakes? | | Learning effectiveness |

## Checklist

- [ ] Learning sources identified and monitored
- [ ] Review cadence established
- [ ] Event retrospective template in use
- [ ] Learning repository created and accessible
- [ ] Action tracking system in place
- [ ] Cross-team sharing mechanisms active
- [ ] Improvement metrics tracked
- [ ] Team trained on learning culture

## Tasks

1. **Audit current learning practices** — what's captured, what's lost?
2. **Establish missing reviews** in your cadence
3. **Create or improve your knowledge base**
4. **Review action completion rate** — are you following through?
5. **Pick one recurring problem** and apply the full learning loop
6. **Celebrate a recent learning** publicly

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# Track B Summary

## Operational Resilience Checklist

Before proceeding to Block 7B (Live Ops & Growth for Mature Games), confirm:

| Element | Complete? | Key Output |
|---------|-----------|------------|
| Risk Register — Live Ops | | Operational risks documented |
| Operational Risk Prioritization | | Readiness levels assigned |
| Economy Exploit Response Plan | | Response playbook ready |
| Server Incident Protocol | | War room protocol defined |
| Negative Review Spike Response | | Monitoring and response plan |
| Rollback Protocol | | Rollback capabilities documented |
| Burnout Early Warning System | | Health monitoring in place |
| Continuous Improvement & Learning | | Learning loop active |

## Key Outputs from Block 6B

| Output | Location | Owner |
|--------|----------|-------|
| Live ops risk register | | |
| Risk prioritization matrix | | |
| Economy exploit playbook | | |
| Incident response protocol | | |
| Review response plan | | |
| Rollback procedures | | |
| Team health dashboard | | |
| Learning repository | | |

## Red Flags Requiring Attention

- [ ] No documented response plans for common incidents
- [ ] Incident response time >1 hour for SEV 1
- [ ] Same incidents recurring without prevention
- [ ] Team health metrics declining
- [ ] On-call burden concentrated on few people
- [ ] No post-mortems conducted recently
- [ ] Learnings not acted upon
- [ ] Rating declining without clear response

---

# Block 6 Complete

## Summary

You've now completed Block 6: Risk & Problem Solving. Whether you're building something new or running a live game, you have frameworks for:

**For Greenfield Projects (Track A):**
- Identifying and tracking development risks
- Prioritizing risks by likelihood and impact
- Reducing key person dependencies
- Monitoring third-party risks
- Preventing crunch before it starts
- Running effective retrospectives
- Conducting blameless post-mortems
- Preserving decision context

**For Mature Games (Track B):**
- Tracking live operational risks
- Preparing appropriate response readiness
- Responding to economy exploits
- Managing server incidents
- Recovering from review spikes
- Rolling back problematic changes
- Protecting team health
- Learning continuously from operations

**Key Principle:** Risk management isn't about avoiding all problems—it's about being ready when problems inevitably occur. Preparation creates calm. Playbooks create speed. Post-mortems create learning. The goal is not zero incidents but rapid, effective response that maintains player trust and team health.

---

*"Hope is not a strategy. Luck is not a factor. Fear is not an option."*  
— James Cameron
