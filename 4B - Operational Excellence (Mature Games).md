---
layout: default
title: "Operational Excellence (Mature Games)"
---
# Operational Excellence (Mature Games)

This track focuses on optimizing existing execution processes for sustained live operations with an emphasis on efficiency, reliability, and continuous improvement.

---

# 4B.1 Execution Process Audit

## Why It Matters

Over time, production processes accumulate cruft—steps that made sense once but no longer do, reviews added after incidents that now slow everything down, workarounds that became permanent. An execution audit reveals inefficiencies and reclaims capacity for player-facing work.

## Framework: Process Inventory

List all recurring execution processes:

| Process | Frequency | Time/Instance | People Involved | Value Add? |
|---------|-----------|---------------|-----------------|------------|
| Event deployment | | | | High/Med/Low |
| Content QA | | | | |
| Bug triage | | | | |
| Config changes | | | | |
| Build process | | | | |
| Release process | | | | |
| | | | | |

**Total time/week on processes:** _______________

## Framework: Value Stream Mapping

For your highest-frequency process, map each step:

| Step | Duration | Wait Time | Who | Value Add? | Necessary? |
|------|----------|-----------|-----|------------|------------|
| 1. | | | | Yes/No | Yes/No |
| 2. | | | | | |
| 3. | | | | | |
| 4. | | | | | |
| 5. | | | | | |
| | | | | | |
| **Total** | | | | | |

**Lead time (total duration):** _______________

**Value-add time (only value-add steps):** _______________

**Efficiency (value-add / lead time):** _______________%

## Framework: Waste Identification

| Waste Type | Found In Your Processes? | Impact | Fix |
|------------|--------------------------|--------|-----|
| **Waiting** | | | |
| **Handoffs** | | | |
| **Rework** | | | |
| **Over-processing** | | | |
| **Motion/switching** | | | |
| **Defects** | | | |
| **Unused talent** | | | |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What process takes longest end-to-end? | | Priority improvement target |
| Where do things wait most often? | | Bottleneck identification |
| Which reviews rarely find issues? | | Candidates for reduction |
| What do people work around? | | Process doesn't match reality |
| What breaks most often? | | Reliability investment needed |

## Framework: Improvement Prioritization

| Improvement | Time Saved | Effort | Risk | Priority |
|-------------|------------|--------|------|----------|
| | hrs/week | S/M/L | Low/Med/High | |
| | | | | |
| | | | | |
| | | | | |

## Checklist

- [ ] All recurring processes inventoried
- [ ] Time spent on each estimated
- [ ] One process value-stream mapped
- [ ] Waste identified
- [ ] Improvements prioritized
- [ ] First improvement scheduled

## Tasks

1. **List all recurring processes** with frequency and time
2. **Value-stream map** your highest-frequency process
3. **Calculate efficiency** (value-add time / total time)
4. **Identify top 3 wastes**
5. **Prioritize one improvement** to implement this month

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4B.2 Definition of Done Refresh

## Why It Matters

DoD created at launch may not fit current reality. The team is different, the game is different, the velocity requirements are different. An outdated DoD either slows things down (excessive requirements) or lets problems through (insufficient requirements). Regular refresh ensures DoD matches current needs.

## Framework: DoD Audit

### Current DoD Assessment

For each DoD criterion, evaluate:

| Criterion | Still Relevant? | Actually Followed? | Should Change? |
|-----------|-----------------|-------------------|----------------|
| | Yes/No | Yes/Partly/No | Remove/Modify/Keep |
| | | | |
| | | | |
| | | | |
| | | | |

### Criteria Causing Friction

| Criterion | Issue | Proposed Solution |
|-----------|-------|-------------------|
| | Takes too long | |
| | Rarely catches issues | |
| | Unclear ownership | |
| | Tools don't support | |

### Missing Criteria

| Gap | Evidence | Proposed Addition |
|-----|----------|-------------------|
| | Issue got through | |
| | Repeated problem | |
| | Industry standard | |

## Framework: DoD by Content Type

Mature games often need different DoD for different content:

| Content Type | DoD Level | Rationale |
|--------------|-----------|-----------|
| Major feature update | Full | High impact, rare |
| Live event (new) | Standard | Regular, meaningful |
| Live event (repeat) | Minimal | Proven, low risk |
| Config change | Targeted | Specific validation |
| Emergency fix | Minimum viable | Speed over completeness |

### Tiered DoD Example

| Tier | When Used | Requirements |
|------|-----------|--------------|
| **Full** | New features, major changes | All standard DoD criteria |
| **Standard** | Regular content | Core criteria only |
| **Minimal** | Repeat content, minor changes | Smoke test + targeted |
| **Emergency** | Hotfix | Fix verified + critical path |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What slips through that shouldn't? | | Missing criteria |
| What takes too long without adding value? | | Remove/streamline |
| What do people skip? | | Irrelevant or unclear |
| What caused recent incidents? | | Gap in DoD |
| What changed since DoD was created? | | May need refresh |

## Checklist

- [ ] Current DoD audited
- [ ] Friction points identified
- [ ] Gaps identified
- [ ] Tiered approach considered
- [ ] Updated DoD documented
- [ ] Team trained on changes

## Tasks

1. **Audit current DoD** with the team
2. **Review last 5 incidents** — would better DoD have caught them?
3. **Identify friction points** — what slows you down without adding value?
4. **Consider tiered approach** for different content types
5. **Document and communicate** updated DoD

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4B.3 Operational Reliability Improvement

## Why It Matters

In live games, reliability is revenue. Every minute of downtime, every broken event, every purchase failure costs real money and player trust. Systematic reliability improvement reduces incidents, speeds recovery, and builds confidence that the game will work when players want to play.

## Framework: Reliability Metrics

| Metric | Current | Target | Industry Benchmark |
|--------|---------|--------|-------------------|
| Uptime % | | 99.9% | 99.9%+ |
| Mean time to detect (MTTD) | | <5 min | <5 min |
| Mean time to respond (MTTR) | | <15 min | <15 min |
| Mean time to resolve | | <1 hour | <2 hours |
| Incidents per month | | <2 | <3 |
| Event success rate | | >99% | >99% |
| Config deployment success | | >99% | >99% |

## Framework: Incident Analysis

Review last 10 incidents:

| Incident | Date | Duration | Impact | Root Cause | Preventable? |
|----------|------|----------|--------|------------|--------------|
| | | | | | Yes/No |
| | | | | | |
| | | | | | |
| | | | | | |

### Root Cause Categories

| Category | Count | % of Incidents | Top Issue |
|----------|-------|----------------|-----------|
| Config error | | | |
| Code bug | | | |
| Infrastructure | | | |
| Third-party | | | |
| Human error | | | |
| Unknown | | | |

## Framework: Reliability Improvement Levers

| Lever | Current State | Improvement | Impact |
|-------|---------------|-------------|--------|
| **Monitoring** | | | |
| Config validation | | Automated checks | Prevent bad configs |
| Alerting coverage | | More metrics | Faster detection |
| Dashboard clarity | | Better visibility | Faster diagnosis |
| **Testing** | | | |
| Staging environment | | More parity | Catch issues early |
| Automated testing | | More coverage | Prevent regressions |
| Canary deployment | | Implement | Limit blast radius |
| **Recovery** | | | |
| Rollback speed | | One-click | Faster resolution |
| Runbook coverage | | Document more | Consistent response |
| On-call readiness | | Better training | Faster response |

## Framework: Error Budget

| Service | Uptime Target | Downtime Budget/Month | Used This Month |
|---------|---------------|----------------------|-----------------|
| Game servers | 99.9% | 43 minutes | |
| Config service | 99.95% | 22 minutes | |
| Purchase flow | 99.99% | 4 minutes | |
| Event system | 99.9% | 43 minutes | |

**When error budget exhausted:** Halt feature work, focus on reliability

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What's our most common incident type? | | Focus prevention efforts |
| How long until we know something's wrong? | | Monitoring gap |
| Can anyone on-call fix any incident? | | Knowledge sharing needed |
| Do we have runbooks for top scenarios? | | Documentation gap |
| When did we last practice incident response? | | Training needed |

## Checklist

- [ ] Reliability metrics defined and tracked
- [ ] Recent incidents analyzed
- [ ] Root causes categorized
- [ ] Improvement levers identified
- [ ] Error budget concept understood
- [ ] Top improvement prioritized

## Tasks

1. **Define reliability metrics** you'll track
2. **Analyze last 10 incidents** for patterns
3. **Identify your biggest reliability gap**
4. **Prioritize one improvement** this month
5. **Establish error budget** concept with leadership

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4B.4 Velocity Optimization

## Why It Matters

Over time, live ops velocity often decreases—more process, more legacy, more caution after incidents. But player expectations increase. Velocity optimization isn't about cutting corners; it's about removing friction so you can deliver more value faster.

## Framework: Velocity Measurement

| Metric | Definition | Current | 6 Months Ago | Trend |
|--------|------------|---------|--------------|-------|
| Event lead time | Idea → live | | | ↑↓→ |
| Content lead time | Ready → deployed | | | |
| Config change lead time | Request → live | | | |
| Bug fix lead time | Reported → deployed | | | |
| Build time | Trigger → complete | | | |
| Deploy time | Approved → live | | | |

**Target:** Decrease lead times by 20%+ while maintaining quality

## Framework: Velocity Blockers

| Blocker Category | Specific Examples | Time Cost | Fix |
|------------------|-------------------|-----------|-----|
| **Approvals** | | | |
| Excessive sign-offs | | | Reduce approvers |
| Slow reviewers | | | Clear SLAs |
| **Testing** | | | |
| Manual testing | | | Automate |
| Environment issues | | | Improve staging |
| **Tooling** | | | |
| Slow builds | | | Optimize/cache |
| Manual deployments | | | CI/CD |
| **Dependencies** | | | |
| Cross-team waits | | | Better planning |
| Third-party delays | | | Decouple |

## Framework: Automation Candidates

| Manual Task | Frequency | Time/Instance | Automation Effort | Priority |
|-------------|-----------|---------------|-------------------|----------|
| | | | S/M/L | |
| | | | | |
| | | | | |
| | | | | |

**ROI Calculation:** (Time saved/month) / (Development effort) = Months to payback

## Framework: Process Streamlining

| Current Process | Steps | Time | Proposed Change | New Time |
|-----------------|-------|------|-----------------|----------|
| | | | | |
| | | | | |

### Streamlining Tactics

| Tactic | When to Apply |
|--------|---------------|
| Remove step | Step rarely finds issues |
| Combine steps | Sequential steps by same person |
| Parallelize | Independent steps in sequence |
| Automate | Repetitive, rule-based |
| Batch | Many small items → fewer large batches |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What takes longest in deployment? | | Optimization target |
| What are you waiting for most often? | | Bottleneck |
| What could be automated that isn't? | | Automation opportunity |
| What process was added after an incident? | | May be over-engineered |
| What would 2x velocity require? | | Stretch target |

## Checklist

- [ ] Velocity metrics defined
- [ ] Current lead times measured
- [ ] Trends analyzed
- [ ] Blockers identified
- [ ] Automation candidates listed
- [ ] Top improvement prioritized

## Tasks

1. **Measure current lead times** for key workflows
2. **Compare to 6 months ago** — are things slower?
3. **Identify top 3 blockers**
4. **Find one automation candidate** with good ROI
5. **Set velocity improvement target** for quarter

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4B.5 Quality Gate Optimization

## Why It Matters

Quality gates exist to catch problems, but too many gates slow everything down while too few let problems through. Optimization means right-sizing gates to actual risk—more scrutiny where it matters, streamlined process where it doesn't.

## Framework: Gate Inventory

List all quality gates in your pipeline:

| Gate | When | Duration | Catch Rate | False Positive Rate |
|------|------|----------|------------|---------------------|
| Code review | | | Issues found/month | Reviews with no issues |
| QA pass | | | | |
| Staging verification | | | | |
| Approval sign-off | | | | |
| | | | | |

### Gate Effectiveness Analysis

| Gate | Issues Caught Last Month | Time Cost | Cost per Issue |
|------|--------------------------|-----------|----------------|
| | | | Time / Issues |
| | | | |
| | | | |

## Framework: Risk-Based Gate Levels

| Risk Level | Criteria | Gates Required |
|------------|----------|----------------|
| **High** | New feature, economy change, major update | Full: Code review + QA + Staging + Approval |
| **Medium** | Content update, balance change | Standard: Code review + QA + Staging |
| **Low** | Repeat content, minor config | Minimal: Automated + Spot check |
| **Emergency** | Hotfix | Fix verification + Smoke test |

### Mapping Content to Risk

| Content Type | Risk Level | Rationale |
|--------------|------------|-----------|
| New feature code | High | High impact, complex |
| New event | Medium | Known patterns, some risk |
| Repeat event | Low | Proven, minimal changes |
| Config tweak | Low-Medium | Depends on change |
| Emergency fix | Per situation | Speed vs. safety trade-off |

## Framework: Gate Optimization Tactics

| Situation | Tactic |
|-----------|--------|
| Gate rarely catches issues | Reduce or remove |
| Gate catches issues but slow | Automate or parallelize |
| Issues slip through gate | Strengthen or add |
| Same issue types repeatedly | Fix root cause, not gate |
| Gate duplicates another | Consolidate |

## Framework: Automated vs. Manual Gates

| Check | Currently | Should Be | Reason |
|-------|-----------|-----------|--------|
| Syntax/compile | | Automated | Fast, deterministic |
| Unit tests | | Automated | Repeatable |
| Schema validation | | Automated | Rule-based |
| Integration test | | Automated | Repeatable |
| Balance sanity | | Automated | Range checks |
| Gameplay feel | | Manual | Subjective |
| Visual quality | | Manual | Judgment needed |
| Player experience | | Manual | Holistic |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| Which gate catches the most issues? | | High-value gate |
| Which gate rarely catches anything? | | Candidate for reduction |
| Where do issues slip through? | | Gap in gates |
| What could be automated? | | Efficiency opportunity |
| What requires human judgment? | | Keep manual |

## Checklist

- [ ] All gates inventoried
- [ ] Effectiveness measured
- [ ] Risk levels defined
- [ ] Content mapped to risk
- [ ] Optimization tactics identified
- [ ] Automation opportunities listed

## Tasks

1. **List all current gates**
2. **Measure effectiveness** (issues caught vs. time spent)
3. **Define risk levels** for your content types
4. **Identify gates to remove/reduce** (low catch rate)
5. **Identify automation opportunities**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4B.6 Tool & Infrastructure Improvement

## Why It Matters

Teams often tolerate bad tools because "that's just how it is." But minutes lost to slow builds, crashed editors, or manual deployments add up to hours per week—hours that could go toward player-facing work. Strategic tool investment pays dividends in velocity and morale.

## Framework: Tool Pain Point Survey

| Tool/System | Pain Points | Impact (hrs/week) | Satisfaction (1-5) |
|-------------|-------------|-------------------|-------------------|
| Build system | | | |
| Deploy system | | | |
| Config management | | | |
| Analytics dashboard | | | |
| Content tools | | | |
| Bug tracking | | | |
| Communication | | | |

### Top Pain Points (Team Survey)

| Pain Point | # Mentions | Impact | Feasibility of Fix |
|------------|------------|--------|-------------------|
| | | | Easy/Med/Hard |
| | | | |
| | | | |
| | | | |

## Framework: Build & Deploy Assessment

| Metric | Current | Target | Industry Benchmark |
|--------|---------|--------|-------------------|
| Build time (CI) | | <10 min | <10 min |
| Build time (full) | | <30 min | <30 min |
| Deploy time | | <5 min | <5 min |
| Rollback time | | <2 min | <2 min |
| Pipeline reliability | | >99% | >99% |

### Build/Deploy Improvement Opportunities

| Improvement | Effort | Time Saved | Priority |
|-------------|--------|------------|----------|
| Incremental builds | | | |
| Build caching | | | |
| Parallel testing | | | |
| One-click deploy | | | |
| Auto-rollback | | | |

## Framework: Content Tool Maturity

| Capability | Level 1 (Manual) | Level 2 (Tool) | Level 3 (Automated) | Current |
|------------|------------------|----------------|---------------------|---------|
| Event creation | Spreadsheet + code | Config UI | Template-based | |
| Offer setup | Manual config | Management UI | Segment-driven | |
| Balance tuning | Code change | Spreadsheet import | Live dashboard | |
| Localization | Manual update | CMS integration | Automated pipeline | |
| A/B test setup | Developer work | Self-serve UI | Automated suggestion | |

## Framework: Infrastructure Investment Prioritization

| Investment | Cost | Impact | Risk | Priority |
|------------|------|--------|------|----------|
| | S/M/L | High/Med/Low | Low/Med/High | |
| | | | | |
| | | | | |
| | | | | |

### ROI Calculation Template

```
Investment: _______________
Cost: _______________ (dev hours)
Time saved: _______________ (hours/week)
Team members affected: _______________
Weekly savings: Time saved × Team members = _______________
Payback period: Cost / Weekly savings = _______________ weeks
```

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| What do people complain about most? | | Top pain point |
| What do people work around? | | Tool doesn't fit need |
| What breaks most often? | | Reliability investment |
| What would 2x speed require? | | Infrastructure gap |
| What do competitors do better? | | Investment opportunity |

## Checklist

- [ ] Tool pain points surveyed
- [ ] Build/deploy metrics measured
- [ ] Content tool maturity assessed
- [ ] Investments prioritized
- [ ] ROI calculated for top priorities
- [ ] Investment plan created

## Tasks

1. **Survey team** on tool pain points
2. **Measure build/deploy times**
3. **Assess content tool maturity**
4. **Prioritize top 3 investments**
5. **Calculate ROI** and build business case

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4B.7 Continuous Improvement Culture

## Why It Matters

One-time improvements decay. Without a culture of continuous improvement, processes accumulate cruft, tools become outdated, and teams accept dysfunction as normal. Building improvement into the rhythm of work creates sustainable excellence.

## Framework: Improvement Mechanisms

| Mechanism | Frequency | Purpose | Owner |
|-----------|-----------|---------|-------|
| **Sprint retrospective** | Per sprint | Process improvement | Scrum Master |
| **Incident post-mortem** | Per incident | Prevent recurrence | Incident owner |
| **Quarterly review** | Quarterly | Strategic improvement | Leadership |
| **Kaizen events** | As needed | Deep-dive on specific issue | Sponsor |
| **Suggestion box** | Ongoing | Surface ideas anytime | Team |

## Framework: Retrospective Evolution

### Basic Retrospective (Starting Point)

| Question | Time | Output |
|----------|------|--------|
| What went well? | 10 min | Celebrate |
| What didn't go well? | 10 min | Issues list |
| What will we try? | 10 min | 1-2 experiments |

### Advanced Retrospective (Mature)

| Question | Time | Output |
|----------|------|--------|
| Review last retro's actions | 5 min | Accountability |
| Data review (metrics) | 5 min | Objective view |
| What helped/hindered? | 10 min | Root causes |
| Improvement experiments | 10 min | Testable changes |
| Assign owners and dates | 5 min | Accountability |

## Framework: Improvement Tracking

| Improvement | Source | Date Identified | Owner | Status | Result |
|-------------|--------|-----------------|-------|--------|--------|
| | Retro/Incident/Other | | | Planned/In progress/Done | Worked/Didn't/Unknown |
| | | | | | |
| | | | | | |

### Improvement Velocity

| Period | Improvements Identified | Improvements Completed | Success Rate |
|--------|------------------------|----------------------|--------------|
| This month | | | |
| Last month | | | |
| Quarter | | | |

## Framework: Learning from Incidents

### Post-Mortem Template

```
INCIDENT: _______________
Date: _______________
Duration: _______________
Impact: _______________

TIMELINE:
_______________________________________________________________________________

ROOT CAUSE:
_______________________________________________________________________________

WHAT WORKED:
_______________________________________________________________________________

WHAT DIDN'T WORK:
_______________________________________________________________________________

ACTION ITEMS:
| Action | Owner | Due | Status |
|--------|-------|-----|--------|
| | | | |
| | | | |

LESSONS:
_______________________________________________________________________________
```

### Post-Mortem Principles

| Principle | Explanation |
|-----------|-------------|
| **Blameless** | Focus on systems, not individuals |
| **Honest** | Capture what really happened |
| **Actionable** | Must result in concrete changes |
| **Shared** | Learnings distributed to team |
| **Followed up** | Actions tracked to completion |

## Framework: Kaizen Event Structure

For deep-dive improvement on specific issue:

| Day | Activity |
|-----|----------|
| **Day 1** | Problem definition, data gathering |
| **Day 2** | Root cause analysis, solution brainstorming |
| **Day 3** | Solution design, pilot implementation |
| **Day 4** | Testing, refinement |
| **Day 5** | Documentation, handoff, celebration |

## Diagnostic Questions

| Question | Answer | Implication |
|----------|--------|-------------|
| When was last improvement implemented? | | Improvement velocity |
| Do retro actions actually happen? | | Follow-through |
| Is same issue raised repeatedly? | | Root cause not addressed |
| Who owns improvement? | | Accountability |
| Is improvement celebrated? | | Cultural reinforcement |

## Checklist

- [ ] Retrospective cadence established
- [ ] Post-mortem process defined
- [ ] Improvement backlog maintained
- [ ] Actions tracked to completion
- [ ] Learnings shared broadly
- [ ] Improvements celebrated

## Tasks

1. **Audit last 5 retrospectives** — how many actions completed?
2. **Review last 5 post-mortems** — are lessons being applied?
3. **Create improvement backlog** as living document
4. **Assign improvement owner** (not additional duty—real responsibility)
5. **Celebrate a recent improvement** publicly

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# Track B Summary

## Operational Excellence Checklist

Before proceeding to Block 5B (Scope Management for Live Games), confirm:

| Element | Complete? | Key Finding |
|---------|-----------|-------------|
| Execution Process Audit | | |
| Definition of Done Refresh | | |
| Operational Reliability Improvement | | |
| Velocity Optimization | | |
| Quality Gate Optimization | | |
| Tool & Infrastructure Improvement | | |
| Continuous Improvement Culture | | |

## Key Outputs from Block 4B

| Output | Location | Owner |
|--------|----------|-------|
| Process efficiency analysis | | |
| Updated DoD | | |
| Reliability improvement plan | | |
| Velocity targets | | |
| Optimized gate structure | | |
| Tool investment roadmap | | |
| Improvement backlog | | |

## Red Flags Requiring Attention

- [ ] Process efficiency <50%
- [ ] DoD not followed or outdated
- [ ] Reliability declining (more incidents)
- [ ] Velocity slowing over time
- [ ] Quality gates creating bottleneck
- [ ] Tool satisfaction <3/5
- [ ] No recent improvements implemented

---

*"How you do anything is how you do everything. Excellence is a habit, not an act."*  
— Adapted from Aristotle

---
