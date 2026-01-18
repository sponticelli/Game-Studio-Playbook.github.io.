---
layout: default
title: "Daily Production and Execution"
---

# Daily Production & Execution

> *"We are what we repeatedly do. Excellence, then, is not an act, but a habit."*  
> — Will Durant (summarizing Aristotle)

---

# TRACK A: Daily Production & Execution (Greenfield Projects)

Complete these topics as you enter production. Return to them when quality slips or execution becomes unpredictable.

---

# 4A.1 Definition of Done — Features

## Why It Matters

"Done" is the most dangerous word in production. Without a shared definition, "done" becomes subjective—engineering thinks it's done when code compiles, QA thinks it's done when testing passes, design thinks it's done when it's fun. This gap creates endless rework cycles, missed deadlines, and finger-pointing. A universal Definition of Done creates shared expectations and prevents the "90% done for 90% of the project" syndrome.

## Framework: Feature Definition of Done Layers

```
┌─────────────────────────────────────────────────────────────────────┐
│                    FEATURE DEFINITION OF DONE                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  LAYER 1: CODE COMPLETE                                     │    │
│  │  • Functionality implemented to spec                        │    │
│  │  • Code reviewed and approved                               │    │
│  │  • Unit tests written and passing                           │    │
│  │  • No compiler warnings                                     │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                           │                                          │
│                           ▼                                          │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  LAYER 2: INTEGRATION COMPLETE                              │    │
│  │  • Merged to main branch                                    │    │
│  │  • Works with all existing systems                          │    │
│  │  • No regressions introduced                                │    │
│  │  • Performance within acceptable range                      │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                           │                                          │
│                           ▼                                          │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  LAYER 3: QA COMPLETE                                       │    │
│  │  • All test cases executed                                  │    │
│  │  • Critical/blocker bugs fixed                              │    │
│  │  • Edge cases validated                                     │    │
│  │  • Signed off by QA                                         │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                           │                                          │
│                           ▼                                          │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │  LAYER 4: RELEASE READY                                     │    │
│  │  • Analytics instrumented                                   │    │
│  │  • Documentation updated                                    │    │
│  │  • Localization complete (if applicable)                    │    │
│  │  • Approved for release                                     │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Universal Feature DoD Checklist

### Code & Implementation

| Criterion | Required | Verified By | Notes |
|-----------|----------|-------------|-------|
| Feature matches design spec | ✓ | Designer | |
| Code compiles without warnings | ✓ | Engineer | |
| Code review completed | ✓ | Peer | |
| Unit tests written and passing | ✓ | Engineer | |
| Edge cases handled | ✓ | Engineer | |
| Error handling implemented | ✓ | Engineer | |
| Memory/performance acceptable | ✓ | Engineer | |

### Integration

| Criterion | Required | Verified By | Notes |
|-----------|----------|-------------|-------|
| Merged to main/develop branch | ✓ | Engineer | |
| Build succeeds | ✓ | CI/CD | |
| No regressions in existing features | ✓ | QA | |
| Works on all target platforms | ✓ | QA | |
| Works with save/load systems | ✓ | QA | |
| Multiplayer sync (if applicable) | ○ | QA | |

### Quality Assurance

| Criterion | Required | Verified By | Notes |
|-----------|----------|-------------|-------|
| Test plan executed | ✓ | QA | |
| All critical bugs fixed | ✓ | QA | |
| All high bugs fixed OR waived | ✓ | QA + Producer | |
| Device/platform matrix tested | ✓ | QA | |
| Certification requirements met | ○ | QA | |
| QA sign-off received | ✓ | QA Lead | |

### Polish & Completion

| Criterion | Required | Verified By | Notes |
|-----------|----------|-------------|-------|
| Final art assets integrated | ✓ | Art | |
| Final audio integrated | ✓ | Audio | |
| UI/UX polish complete | ✓ | Designer | |
| Animations at final quality | ✓ | Animator | |
| VFX at final quality | ✓ | VFX Artist | |

### Data & Analytics

| Criterion | Required | Verified By | Notes |
|-----------|----------|-------------|-------|
| Analytics events instrumented | ✓ | Engineer | |
| Economy transactions tracked | ○ | Engineer | |
| Funnel points captured | ✓ | Analytics | |
| A/B test hooks (if applicable) | ○ | Engineer | |
| Data validated in staging | ✓ | Analytics | |

### Documentation & Handoff

| Criterion | Required | Verified By | Notes |
|-----------|----------|-------------|-------|
| Release notes written | ✓ | PM/Producer | |
| Config documentation updated | ✓ | Engineer | |
| Known issues documented | ✓ | QA | |
| Support team briefed | ○ | PM | |
| Localization complete | ○ | Localization | |

**Legend:** ✓ = Always required | ○ = Required if applicable

## Framework: Role-Specific DoD Additions

| Role | Additional Criteria |
|------|---------------------|
| **Designer** | Balancing validated, gameplay feel approved, tutorial coverage |
| **Artist** | Assets meet style guide, proper naming conventions, LODs created |
| **Engineer** | Tech debt documented, code commented, debugging tools available |
| **QA** | Test cases archived, repro steps documented, device coverage noted |
| **Producer** | Stakeholder demo completed, risks communicated, schedule updated |

## Framework: Your Feature DoD Template

Use this to create your project-specific Definition of Done:

| Category | Criterion | Required? | Verified By |
|----------|-----------|-----------|-------------|
| **Code** | | | |
| | | | |
| | | | |
| **Integration** | | | |
| | | | |
| | | | |
| **QA** | | | |
| | | | |
| | | | |
| **Polish** | | | |
| | | | |
| | | | |
| **Data** | | | |
| | | | |
| **Documentation** | | | |
| | | | |

## Checklist

- [ ] Definition of Done documented
- [ ] All disciplines contributed and agreed
- [ ] DoD is visible to all team members
- [ ] Tracking system reflects DoD criteria
- [ ] Process for updating DoD established
- [ ] Everyone understands when to invoke DoD

## Tasks

1. **Draft your DoD** using the templates above
2. **Review with each discipline** — get explicit agreement
3. **Integrate into tracking system** — tasks can't close without DoD
4. **Post it visibly** — physical board or shared doc
5. **Test it** on the next 3 features, then refine

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.2 Definition of Done — Live Content

## Why It Matters

Live content moves faster than features but has higher stakes—a broken event costs real revenue and player trust immediately. Unlike features that can be patched, live content often has fixed windows: a holiday event that launches broken can't be "fixed in post." A Live Content DoD is your quality gate before anything touches production.

## Framework: Live Content DoD Categories

```
┌─────────────────────────────────────────────────────────────────────┐
│                    LIVE CONTENT CATEGORIES                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐ │
│  │   EVENTS    │  │   OFFERS    │  │   CONFIGS   │  │   CONTENT   │ │
│  │             │  │             │  │             │  │   UPDATES   │ │
│  │ Time-limited│  │ Purchases,  │  │ Balance,    │  │ New levels, │ │
│  │ gameplay    │  │ bundles,    │  │ difficulty, │  │ characters, │ │
│  │ experiences │  │ sales       │  │ economy     │  │ items       │ │
│  └─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘ │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Event DoD Checklist

### Pre-Deployment (48+ Hours Before)

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Event spec finalized and approved | Designer | ☐ |
| All assets created and integrated | Art Lead | ☐ |
| Rewards and economy reviewed | Economy | ☐ |
| Localization complete (all languages) | Loc Manager | ☐ |
| Event configured in staging | Live Ops | ☐ |
| Staging playthrough completed | QA | ☐ |

### QA Validation (24-48 Hours Before)

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Event start/end times verified | QA | ☐ |
| All event mechanics functional | QA | ☐ |
| Reward distribution working | QA | ☐ |
| Leaderboards/rankings functional (if applicable) | QA | ☐ |
| Edge cases tested (timezone, reinstall, etc.) | QA | ☐ |
| Performance acceptable | QA | ☐ |
| No critical/blocker bugs | QA Lead | ☐ |

### Final Checks (Day Before)

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Config promoted to production (inactive) | Live Ops | ☐ |
| Activation time confirmed | Live Ops | ☐ |
| Push notification scheduled | Marketing | ☐ |
| Social/community announcement ready | Community | ☐ |
| Support briefed on event | Support Lead | ☐ |
| Rollback plan documented | Live Ops | ☐ |
| Monitoring dashboard ready | Analytics | ☐ |

### Go-Live Criteria

| Criterion | Required | Verified By |
|-----------|----------|-------------|
| All QA validation items passed | ✓ | QA Lead |
| All final check items complete | ✓ | Live Ops Lead |
| No blocking issues in production | ✓ | Engineering |
| Stakeholder approval received | ✓ | Producer |

## Framework: Offer/Purchase DoD Checklist

### Configuration

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Price correct in all currencies | Economy | ☐ |
| Contents/rewards correct | Designer | ☐ |
| Art assets correct and sized | Art | ☐ |
| Localized text correct | Localization | ☐ |
| Purchase limits set correctly | Economy | ☐ |
| Targeting/segments configured | Live Ops | ☐ |

### Validation

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Purchase flow tested (real money in staging) | QA | ☐ |
| Rewards granted correctly | QA | ☐ |
| Purchase tracked in analytics | Analytics | ☐ |
| Receipt validation working | Engineering | ☐ |
| Refund scenario tested | QA | ☐ |
| Edge cases (offline, interrupt) tested | QA | ☐ |

### Compliance

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Pricing meets store requirements | Producer | ☐ |
| No loot box regulation violations | Legal/Producer | ☐ |
| Age-appropriate content | Producer | ☐ |

## Framework: Config Change DoD Checklist

### Balance/Economy Changes

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Change request documented | Designer | ☐ |
| Impact analysis completed | Economy | ☐ |
| Tested in staging environment | QA | ☐ |
| No unintended side effects | QA | ☐ |
| Analytics tracking config change | Analytics | ☐ |
| Rollback values documented | Live Ops | ☐ |
| Communication plan (if player-facing) | Community | ☐ |

## Framework: Content Update DoD Checklist

### New Levels/Characters/Items

| Criterion | Verified By | Sign-off |
|-----------|-------------|----------|
| Design spec approved | Lead Designer | ☐ |
| All assets final quality | Art Lead | ☐ |
| Implementation complete | Engineering | ☐ |
| Balance validated | Economy/Design | ☐ |
| Localization complete | Localization | ☐ |
| Full QA pass completed | QA Lead | ☐ |
| Analytics instrumented | Analytics | ☐ |
| Unlock/acquisition path verified | QA | ☐ |

## Framework: Live Content Staging Gate

```
┌─────────────────────────────────────────────────────────────────────┐
│                    STAGING GATE PROCESS                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│     CONTENT           STAGING           VALIDATION          PROD   │
│     CREATION          DEPLOY            PERIOD              DEPLOY │
│                                                                     │
│  ┌──────────┐      ┌──────────┐      ┌──────────┐      ┌──────────┐│
│  │ Complete │ ───► │ Deploy   │ ───► │ QA Test  │ ───► │ Promote  ││
│  │ Content  │      │ to       │      │ 24-48    │      │ to       ││
│  │          │      │ Staging  │      │ hours    │      │ Live     ││
│  └──────────┘      └──────────┘      └──────────┘      └──────────┘│
│                                            │                       │
│                                            ▼                       │
│                                    ┌──────────────┐                │
│                                    │   BLOCKER?   │                │
│                                    │  ┌───┐ ┌───┐ │                │
│                                    │  │Yes│ │No │ │                │
│                                    │  └─┬─┘ └─┬─┘ │                │
│                                    └────┼─────┼───┘                │
│                                         │     │                    │
│                                         ▼     ▼                    │
│                                    ┌─────┐ ┌──────┐                │
│                                    │Fix &│ │Approve│                │
│                                    │Retry│ │Deploy │                │
│                                    └─────┘ └──────┘                │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Staging Validation Checklist

| Category | Test | Pass? |
|----------|------|-------|
| **Functional** | Core mechanic works | ☐ |
| | Rewards granted correctly | ☐ |
| | UI displays properly | ☐ |
| | Timers/countdowns accurate | ☐ |
| **Data** | Analytics events firing | ☐ |
| | Economy transactions logging | ☐ |
| **Performance** | Load times acceptable | ☐ |
| | No memory leaks | ☐ |
| | Frame rate stable | ☐ |
| **Edge Cases** | Timezone transitions | ☐ |
| | Session resume | ☐ |
| | Offline handling | ☐ |

## Checklist

- [ ] Live Content DoD documented
- [ ] Staging environment available
- [ ] QA process for live content defined
- [ ] Minimum validation period established
- [ ] Rollback procedures documented
- [ ] All roles understand their sign-off responsibilities

## Tasks

1. **Customize DoD checklists** for your content types
2. **Set up staging environment** that mirrors production
3. **Define minimum validation periods** (24h? 48h?)
4. **Create sign-off workflow** in your tools
5. **Train team** on live content process

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.3 Multi-Level Done Framework

## Why It Matters

Not everything needs to be polished. Prototypes shouldn't have final UI. Early features shouldn't block on localization. But without clarity on "how done is done enough," teams either over-invest (polishing throwaway work) or under-invest (shipping rough work as final). A multi-level Done framework matches investment to purpose.

## Framework: The Four Levels of Done

```
┌─────────────────────────────────────────────────────────────────────┐
│                    MULTI-LEVEL DONE FRAMEWORK                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  D1: WORKS              "Does the thing function?"                  │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │ • Core functionality implemented                            │    │
│  │ • Can be tested/evaluated                                   │    │
│  │ • Placeholder assets acceptable                             │    │
│  │ • Known bugs acceptable                                     │    │
│  │ • NOT integrated with other systems                         │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                           │                                          │
│                           ▼                                          │
│  D2: INTEGRATED          "Does it work WITH everything else?"       │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │ • Works in context of full game                             │    │
│  │ • Connected to relevant systems                             │    │
│  │ • WIP assets (not final)                                    │    │
│  │ • Major bugs fixed                                          │    │
│  │ • Performance may be rough                                  │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                           │                                          │
│                           ▼                                          │
│  D3: POLISHED            "Is it good enough to show externally?"    │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │ • Final or near-final assets                                │    │
│  │ • UI polished                                               │    │
│  │ • No obvious bugs                                           │    │
│  │ • Performance acceptable                                    │    │
│  │ • Could be shown to players/press                           │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                           │                                          │
│                           ▼                                          │
│  D4: SHIPPABLE           "Is it ready for production release?"      │
│  ┌─────────────────────────────────────────────────────────────┐    │
│  │ • Full Definition of Done met                               │    │
│  │ • QA signed off                                             │    │
│  │ • Localized                                                 │    │
│  │ • Analytics instrumented                                    │    │
│  │ • Documentation complete                                    │    │
│  └─────────────────────────────────────────────────────────────┘    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Level-Specific Criteria

### D1: Works

| Aspect | Requirement | Example |
|--------|-------------|---------|
| **Code** | Functional, compilable | Feature can be triggered |
| **Art** | Placeholder acceptable | Gray boxes, borrowed assets |
| **Audio** | Silent or placeholder | Stock sounds OK |
| **UI** | Functional only | Buttons work, no styling |
| **QA** | Self-tested | Dev confirms it works |
| **Bugs** | Crash-free | Non-crashes acceptable |

**Use D1 for:** Prototypes, proof of concepts, internal evaluation, "can we do this?"

### D2: Integrated

| Aspect | Requirement | Example |
|--------|-------------|---------|
| **Code** | Works with other systems | Save/load, progression, economy |
| **Art** | WIP but directional | Rough animations, temp colors |
| **Audio** | Temp implementation | Placeholder SFX/music |
| **UI** | Styled but not final | Correct layout, temp graphics |
| **QA** | Tested in context | Feature regression test |
| **Bugs** | Critical fixed | Major bugs noted |

**Use D2 for:** Alpha milestone, internal playtests, stakeholder reviews, vertical slice components

### D3: Polished

| Aspect | Requirement | Example |
|--------|-------------|---------|
| **Code** | Optimized, stable | No performance issues |
| **Art** | Final or near-final | May need minor tweaks |
| **Audio** | Final implementation | Correct sounds in place |
| **UI** | Polished | Animations, feedback, juice |
| **QA** | Full test pass | Bug count low |
| **Bugs** | High/critical fixed | Only minor bugs remain |

**Use D3 for:** Beta milestone, external playtests, press demos, soft launch

### D4: Shippable

| Aspect | Requirement | Example |
|--------|-------------|---------|
| **Code** | Release-ready | Certified if required |
| **Art** | Final, approved | All assets delivered |
| **Audio** | Final, mixed | Levels balanced |
| **UI** | Localized, accessible | All languages, settings |
| **QA** | Signed off | Test complete |
| **Bugs** | Known issues acceptable | Ship with list |
| **Analytics** | Instrumented | All events tracking |
| **Docs** | Complete | Support/release ready |

**Use D4 for:** Global launch, live content release, client updates

## Framework: Phase-to-Level Mapping

| Project Phase | Target Done Level | Notes |
|---------------|-------------------|-------|
| Prototype | D1 | Speed over quality |
| Vertical Slice | D3 (for slice content) | Demonstrable quality |
| Alpha | D2 (most features) | Integration focus |
| Beta | D3 (all features) | Polish focus |
| Release Candidate | D4 (all features) | Ship ready |
| Live Content | D4 | Always shippable |

## Framework: Work Item Level Tagging

Add done level to every work item:

| Task | Current Level | Target Level | Gap Work |
|------|---------------|--------------|----------|
| Combat system | D2 | D3 | Polish pass, final VFX |
| Inventory UI | D1 | D3 | Integration, assets, QA |
| Tutorial | D2 | D4 | Localization, analytics |
| Event #1 | D3 | D4 | QA sign-off, docs |

## Framework: Level Progression Tracking

```
FEATURE: _______________

┌──────────────────────────────────────────────────────────────┐
│ D1 │████████████████████████████│ Complete: 2024-01-15     │
├──────────────────────────────────────────────────────────────┤
│ D2 │██████████████████          │ Complete: 2024-02-01     │
├──────────────────────────────────────────────────────────────┤
│ D3 │████████                    │ Target: 2024-02-28       │
├──────────────────────────────────────────────────────────────┤
│ D4 │                            │ Target: 2024-03-15       │
└──────────────────────────────────────────────────────────────┘
```

## Checklist

- [ ] Four levels defined with clear criteria
- [ ] Phase-to-level mapping documented
- [ ] Work items tagged with current/target levels
- [ ] Team understands when each level is appropriate
- [ ] Tracking system supports level tagging
- [ ] Reviews check for level-appropriate work

## Tasks

1. **Customize level criteria** for your project's specifics
2. **Tag existing work items** with current and target levels
3. **Review backlog** — are targets appropriate for each phase?
4. **Train team** on level expectations
5. **Add level discussion** to planning and review meetings

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.4 Task Breakdown Standards

## Why It Matters

"Build the combat system" is not a task—it's a month of work masquerading as a checkbox. Large tasks hide complexity, make estimation impossible, prevent progress visibility, and create "it's almost done" purgatory. Right-sized tasks enable accurate tracking, early problem detection, and the psychological benefit of regular completion.

## Framework: Task Size Guidelines

```
┌─────────────────────────────────────────────────────────────────────┐
│                    TASK SIZE SPECTRUM                               │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  TOO SMALL                IDEAL                     TOO LARGE       │
│  (<1 hour)              (2-8 hours)               (>2 days)        │
│                                                                     │
│  ┌─────────┐          ┌─────────────┐          ┌─────────────┐     │
│  │• "Fix   │          │• "Implement │          │• "Build     │     │
│  │  typo"  │          │  jump       │          │  combat     │     │
│  │• "Update│          │  mechanic"  │          │  system"    │     │
│  │  color" │          │• "Create    │          │• "Create    │     │
│  │• "Rename│          │  enemy AI   │          │  all        │     │
│  │  file"  │          │  patrol"    │          │  enemies"   │     │
│  └─────────┘          └─────────────┘          └─────────────┘     │
│                                                                     │
│  Problems:              Benefits:               Problems:           │
│  • Tracking overhead    • Trackable progress   • Hidden complexity  │
│  • No meaningful        • Estimable            • "Almost done"      │
│  • Groups into noise    • Completable in day   • No visibility      │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: The One-Day Rule

**Target:** Tasks should be completable in one working day or less.

| Duration | Classification | Action |
|----------|---------------|--------|
| < 1 hour | Too small | Batch with related work |
| 1-4 hours | Small | Good for quick wins |
| 4-8 hours | Ideal | Standard task size |
| 1-2 days | Acceptable | Break down if possible |
| 2-5 days | Too large | Must break down |
| > 5 days | Epic | Definitely break down |

## Framework: Task Breakdown Techniques

### Vertical Slicing (Preferred)

Break by deliverable value, not by discipline:

```
BAD (Horizontal):                 GOOD (Vertical):
┌───────────────────────┐         ┌───────────────────────┐
│ "Enemy system"        │         │ "Basic enemy moves"   │
│                       │         │ (1 enemy, patrol only)│
│ 1. Enemy AI (5 days)  │         ├───────────────────────┤
│ 2. Enemy art (5 days) │         │ "Enemy attacks"       │
│ 3. Enemy sound (2 days│         │ (add attack behavior) │
│ 4. Enemy integration  │         ├───────────────────────┤
│    (3 days)           │         │ "Enemy variety"       │
│                       │         │ (add 2nd enemy type)  │
└───────────────────────┘         └───────────────────────┘

Problem: Nothing playable      Benefit: Playable at each step
until all 4 done               Can stop anytime with value
```

### INVEST Criteria

Good tasks are:

| Letter | Criterion | Question |
|--------|-----------|----------|
| **I** | Independent | Can be done without waiting for other tasks? |
| **N** | Negotiable | Scope can be adjusted if needed? |
| **V** | Valuable | Delivers value when complete? |
| **E** | Estimable | Can be reasonably estimated? |
| **S** | Small | Can be completed in days, not weeks? |
| **T** | Testable | Can verify when done? |

### Breakdown Questions

When a task is too large, ask:

| Question | Example Breakdown |
|----------|-------------------|
| Can this be split by **feature subset**? | "All enemies" → "Basic enemy" + "Boss enemy" |
| Can this be split by **iteration**? | "Inventory system" → "Basic inventory" + "Inventory UI" + "Inventory persistence" |
| Can this be split by **platform**? | "Input system" → "Keyboard input" + "Controller input" |
| Can this be split by **workflow step**? | "Character" → "Character model" + "Character rig" + "Character animation" |
| Can this be split by **risk**? | "New tech" → "Tech spike" + "Tech implementation" |

## Framework: Task Anatomy Template

Every task should have:

| Component | Description | Example |
|-----------|-------------|---------|
| **Title** | Action + Object | "Implement double-jump mechanic" |
| **Description** | What and why | "Add ability for player to jump again mid-air" |
| **Acceptance Criteria** | How we know it's done | "Player can jump twice, height configurable" |
| **Estimate** | Expected duration | "4 hours" |
| **Dependencies** | What's blocking | "Requires: Basic jump complete" |
| **Done Level** | Target done state | "D2: Integrated" |

### Example Well-Written Tasks

**Good:**
```
Title: Implement enemy patrol behavior
Description: Enemy walks between waypoints at configurable speed
Acceptance Criteria:
- Enemy follows waypoint path
- Speed adjustable in editor
- Loops or ping-pongs based on setting
- Stops and idles at each waypoint
Estimate: 6 hours
Dependencies: Basic enemy movement
Done Level: D2
```

**Bad:**
```
Title: Enemy AI
Description: Make enemies work
Estimate: ???
```

## Framework: Breaking Down a Large Feature

### Example: "Combat System"

**Step 1:** List components
- Player attack
- Enemy attack
- Damage calculation
- Health/death
- Hit feedback
- Combat UI

**Step 2:** Find minimum viable slice
- Player can attack (D1)
- Enemy takes damage and dies (D1)

**Step 3:** Create incremental tasks

| Task | Size | Depends On |
|------|------|------------|
| Basic player attack animation trigger | 4h | - |
| Attack hitbox detection | 4h | Attack trigger |
| Enemy damage and death | 4h | Hitbox |
| Health UI display | 3h | Enemy damage |
| Enemy attack behavior | 6h | Enemy damage |
| Player takes damage | 4h | Enemy attack |
| Hit VFX and sound | 4h | Hitbox |
| Damage numbers | 3h | Damage |

## Checklist

- [ ] Task size guidelines defined
- [ ] Team trained on breakdown techniques
- [ ] Task template in use
- [ ] Large tasks flagged in tracking system
- [ ] Regular task review in planning
- [ ] Acceptance criteria required

## Tasks

1. **Audit current backlog** — flag tasks > 2 days
2. **Break down flagged tasks** using vertical slicing
3. **Create task template** in your tracking system
4. **Train team** on INVEST criteria
5. **Add task size check** to sprint planning

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.5 Work-in-Progress Limits

## Why It Matters

Context switching is expensive—studies show it costs 20-40% of productive time. When team members juggle too many tasks, everything slows down, quality drops, and nothing gets finished. WIP limits force completion before starting new work, reducing multitasking overhead and increasing flow.

## Framework: The Cost of Multitasking

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CONTEXT SWITCHING COST                           │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  Simultaneous Projects    % Time Lost to Switching                  │
│                                                                     │
│         1                        0%  ████████████████████████████   │
│         2                       20%  ████████████████████           │
│         3                       40%  ████████████████               │
│         4                       60%  ████████████                   │
│         5                       75%  ██████████                     │
│                                                                     │
│  Source: Gerald Weinberg, "Quality Software Management"             │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: WIP Limit Levels

### Individual Limits

| Role | Recommended WIP | Rationale |
|------|-----------------|-----------|
| Engineer | 1-2 items | Deep focus needed |
| Designer | 2-3 items | Mix of creation and review |
| Artist | 2-3 items | Pipeline stages |
| QA | 3-5 items | Testing batches |
| Producer | 3-5 items | Coordination role |

### Team Limits

| Team Size | Total WIP Limit | Rule of Thumb |
|-----------|-----------------|---------------|
| 3-5 | 5-8 | ~1.5x team size |
| 6-10 | 8-12 | ~1.2x team size |
| 11-15 | 12-18 | ~1.1x team size |
| 15+ | Consider splitting | Too large for one kanban |

### Column Limits (Kanban)

```
┌─────────────────────────────────────────────────────────────────────┐
│                    KANBAN BOARD WITH WIP LIMITS                     │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  TO DO          IN PROGRESS      IN REVIEW         DONE            │
│  (No limit)     (Limit: 6)       (Limit: 4)       (No limit)       │
│                                                                     │
│  ┌─────┐        ┌─────┐          ┌─────┐          ┌─────┐          │
│  │     │        │ ██  │          │ ██  │          │     │          │
│  │ ██  │        │ ██  │          │ ██  │          │ ██  │          │
│  │ ██  │        │ ██  │          │ ██  │          │ ██  │          │
│  │ ██  │        │ ██  │          │     │          │ ██  │          │
│  │ ██  │        │ ██  │          └─────┘          │ ██  │          │
│  │ ██  │        │ ██  │          (2 of 4)         │ ██  │          │
│  └─────┘        └─────┘                           └─────┘          │
│  (Backlog)      (6 of 6 = FULL)                                    │
│                                                                     │
│  When "In Progress" hits limit:                                     │
│  → Help finish existing work before starting new                    │
│  → Pull from "In Review" if blocked                                 │
│  → Swarm on blockers                                                │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Stop Starting, Start Finishing

When WIP limit is hit:

| Priority | Action |
|----------|--------|
| **1st** | Help someone else finish their work |
| **2nd** | Review/unblock items in review |
| **3rd** | Fix bugs in current sprint |
| **4th** | Reduce technical debt |
| **5th** | Prepare for upcoming work |
| **Last** | Start new work (only if nothing else possible) |

## Framework: Calculating Your WIP Limit

### Formula Approach

```
WIP Limit = (Desired Throughput) × (Average Cycle Time)

Example:
- Want to complete 10 items per week
- Average item takes 3 days
- WIP Limit = 10 × (3/5) = 6 items
```

### Empirical Approach

1. Start with limit = team size × 1.5
2. Track cycle time for 2 weeks
3. If cycle time increases → lower WIP
4. If team is idle waiting → raise WIP slightly
5. Find equilibrium

## Framework: WIP Limit Violations

| Situation | Response |
|-----------|----------|
| Urgent production bug | Allowed to exceed temporarily, but stop other work |
| "Just one more thing" | Not allowed—finish something first |
| Waiting on external | Can start new if truly blocked AND documented |
| Manager pressure | Explain cost, show data |

### Tracking Violations

| Date | Reason | Duration | Impact |
|------|--------|----------|--------|
| | | | |
| | | | |

**Violation patterns reveal:** process problems, unrealistic limits, or external pressures

## Framework: Your WIP Limits

| Level | Limit | Current State |
|-------|-------|---------------|
| **Personal** | | |
| Engineer A | | |
| Engineer B | | |
| Designer | | |
| Artist | | |
| **Team** | | |
| In Progress column | | |
| In Review column | | |
| **Project** | | |
| Active features | | |
| Active bug fixes | | |

## Checklist

- [ ] Individual WIP limits set
- [ ] Team/column WIP limits set
- [ ] Tracking system enforces limits
- [ ] Team trained on limit responses
- [ ] Violation process defined
- [ ] Regular limit review scheduled

## Tasks

1. **Calculate initial limits** using team size formula
2. **Configure tracking system** to show/enforce limits
3. **Train team** on "stop starting, start finishing"
4. **Track cycle time** for 2 weeks
5. **Adjust limits** based on data

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.6 Blocker Identification & Escalation

## Why It Matters

A blocked task often means an idle person—burning budget while making zero progress. Blockers that aren't surfaced quickly compound: what could have been solved with a 5-minute conversation becomes a week of waiting. Early identification and speed-appropriate escalation keeps work flowing.

## Framework: Blocker Categories

```
┌─────────────────────────────────────────────────────────────────────┐
│                    BLOCKER TAXONOMY                                 │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────────────┐  ┌─────────────────────┐                   │
│  │  TECHNICAL          │  │  DEPENDENCY         │                   │
│  │                     │  │                     │                   │
│  │  • Bug in system    │  │  • Waiting for      │                   │
│  │  • Missing tool     │  │    another task     │                   │
│  │  • Tech limitation  │  │  • External API     │                   │
│  │  • Build broken     │  │  • Asset not ready  │                   │
│  └─────────────────────┘  └─────────────────────┘                   │
│                                                                     │
│  ┌─────────────────────┐  ┌─────────────────────┐                   │
│  │  DECISION           │  │  RESOURCE           │                   │
│  │                     │  │                     │                   │
│  │  • Need approval    │  │  • Person unavail.  │                   │
│  │  • Unclear spec     │  │  • Hardware missing │                   │
│  │  • Conflicting      │  │  • License needed   │                   │
│  │    requirements     │  │  • Budget approval  │                   │
│  └─────────────────────┘  └─────────────────────┘                   │
│                                                                     │
│  ┌─────────────────────┐  ┌─────────────────────┐                   │
│  │  INFORMATION        │  │  EXTERNAL           │                   │
│  │                     │  │                     │                   │
│  │  • Missing context  │  │  • Platform issue   │                   │
│  │  • Question needs   │  │  • Vendor delay     │                   │
│  │    answering        │  │  • Certification    │                   │
│  │  • Docs unclear     │  │  • Legal review     │                   │
│  └─────────────────────┘  └─────────────────────┘                   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Blocker Severity Levels

| Level | Definition | Example | Response |
|-------|------------|---------|----------|
| **Soft** | Slowed but can work around | Waiting for final art, using placeholder | Continue with workaround |
| **Hard** | Fully stopped, no workaround | Dependent feature not done | Escalate immediately |
| **Critical** | Blocking multiple people/features | Build broken, server down | War room/emergency |

## Framework: Escalation Path & Timing

```
┌─────────────────────────────────────────────────────────────────────┐
│                    ESCALATION LADDER                                │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  TIME BLOCKED    ACTION                          WHO INVOLVED       │
│                                                                     │
│  0-30 min        Try to self-solve               You                │
│      │                                                              │
│      ▼                                                              │
│  30 min - 2h     Ask teammate/slack channel      Team               │
│      │                                                              │
│      ▼                                                              │
│  2-4 hours       Raise in standup or to lead     Lead + Team        │
│      │                                                              │
│      ▼                                                              │
│  4-8 hours       Escalate to Producer/Manager    Producer           │
│      │                                                              │
│      ▼                                                              │
│  1+ day          Executive escalation            Director/VP        │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Critical Blockers (Immediate Escalation)

| Blocker Type | Escalate Immediately To |
|--------------|------------------------|
| Build broken | Engineering Lead |
| Server/infrastructure down | Operations/Devops |
| Legal/compliance issue | Producer → Legal |
| Security incident | Security + Leadership |
| Multiple people blocked | Producer |

## Framework: Blocker Documentation

When reporting a blocker:

| Field | Content | Example |
|-------|---------|---------|
| **What** | Specific task blocked | "Inventory UI implementation" |
| **Why** | Root cause | "Backend API not returning correct data" |
| **Since When** | Duration | "Since yesterday 2pm" |
| **Impact** | What's affected | "Can't test inventory flow, QA idle" |
| **Tried** | Self-resolution attempts | "Asked in Slack, checked docs" |
| **Need** | Specific help required | "Backend engineer to fix API" |
| **Workaround?** | Temporary solution | "Can mock data for now" |

### Blocker Template (For Tracking System)

```
BLOCKER: [Task Name] blocked by [Brief Description]
Type: Technical / Dependency / Decision / Resource / Information / External
Severity: Soft / Hard / Critical
Since: [Date/Time]
Impact: [Who/what is affected]
Need: [Specific request]
Owner: [Who's responsible for resolution]
```

## Framework: Daily Blocker Surfacing

### Stand-up Blocker Protocol

| Timing | Action |
|--------|--------|
| **Before standup** | Update blocker status in tracking |
| **During standup** | State blockers clearly (not "might need help") |
| **After standup** | Blocker owners meet to resolve |

### Blocker Board

```
┌─────────────────────────────────────────────────────────────────────┐
│                    ACTIVE BLOCKERS                                  │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  🔴 CRITICAL (0)                                                    │
│  ├── (none)                                                         │
│                                                                     │
│  🟠 HARD (2)                                                        │
│  ├── Backend API - Owner: Sarah - Since: Mon - ETA: Today          │
│  └── Art approval - Owner: Mike - Since: Tue - ETA: Wed            │
│                                                                     │
│  🟡 SOFT (3)                                                        │
│  ├── Final audio - Owner: Audio team - Workaround in place         │
│  ├── Localization - Owner: Loc vendor - Expected Fri               │
│  └── Design question - Owner: Lead Designer - Asked, waiting       │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Blocker Resolution Tracking

| Blocker | Type | Raised | Resolved | Duration | Resolution |
|---------|------|--------|----------|----------|------------|
| | | | | | |
| | | | | | |

**Metrics to track:**
- Average time to resolution by type
- Repeat blockers (systemic issues)
- Escalation frequency
- Impact hours lost

## Checklist

- [ ] Blocker categories defined
- [ ] Severity levels clear to team
- [ ] Escalation path documented
- [ ] Timing thresholds agreed
- [ ] Blocker template in tracking system
- [ ] Daily surfacing process in standup
- [ ] Resolution tracking in place

## Tasks

1. **Create blocker template** in your tracking system
2. **Document escalation contacts** and response times
3. **Train team** on severity classification
4. **Add "blockers" section** to standup agenda
5. **Review blocker metrics** weekly to find patterns

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.7 Build Stability Standards

## Why It Matters

A broken build blocks everyone. When the main branch doesn't compile or run, all integration stops, testing halts, and frustration builds. Build stability is the foundation of team productivity—protecting it with standards and automation prevents cascading delays.

## Framework: Build Stability Tiers

```
┌─────────────────────────────────────────────────────────────────────┐
│                    BUILD STABILITY PYRAMID                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                         ┌─────────┐                                 │
│                         │ RELEASE │  Certified, store-ready        │
│                         │  BUILD  │  (Weekly/Milestone)            │
│                      ┌──┴─────────┴──┐                              │
│                      │  DAILY BUILD  │  Playable, testable          │
│                      │               │  (Every night)               │
│                   ┌──┴───────────────┴──┐                           │
│                   │    CONTINUOUS       │  Compiles, basic tests    │
│                   │    INTEGRATION      │  (Every commit)           │
│                ┌──┴─────────────────────┴──┐                        │
│                │      LOCAL BUILD         │  Developer machine       │
│                │                          │  (Constant)              │
│                └──────────────────────────┘                         │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Green Build Requirements by Tier

### Continuous Integration (Every Commit)

| Requirement | Check | Failure Response |
|-------------|-------|------------------|
| Code compiles | Automated | Block merge |
| No compiler warnings (critical) | Automated | Block merge |
| Unit tests pass | Automated | Block merge |
| Static analysis passes | Automated | Block merge |
| Build time < X minutes | Automated | Alert |

### Daily Build (Every Night)

| Requirement | Check | Failure Response |
|-------------|-------|------------------|
| All CI requirements | Automated | Alert team |
| Game launches | Automated smoke test | P1 bug |
| Core loop playable | Automated or manual | P1 bug |
| No critical crashes | Crash reporting | P1 bug |
| All platforms build | Automated | P1 bug |
| Performance within bounds | Automated | P2 bug |

### Release Build (Weekly/Milestone)

| Requirement | Check | Failure Response |
|-------------|-------|------------------|
| All daily build requirements | Automated | Block release |
| Full test suite passes | Automated + manual | Fix or waive |
| Performance targets met | Profiling | Fix required |
| Memory targets met | Analysis | Fix required |
| No known critical bugs | Bug database | Fix or defer |
| Platform certification checks | Manual/automated | Fix required |

## Framework: Build Break Protocol

```
┌─────────────────────────────────────────────────────────────────────┐
│                    BUILD BREAK RESPONSE                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  BUILD BREAKS                                                       │
│       │                                                             │
│       ▼                                                             │
│  ┌─────────────────┐                                                │
│  │ Automated Alert │ → Slack/Email/Dashboard                        │
│  └────────┬────────┘                                                │
│           │                                                         │
│           ▼                                                         │
│  ┌─────────────────┐     ┌─────────────────┐                        │
│  │ Identify Cause  │ ──► │ Recent Commits  │                        │
│  └────────┬────────┘     │ Changed Files   │                        │
│           │              └─────────────────┘                        │
│           ▼                                                         │
│  ┌─────────────────────────────────────────┐                        │
│  │ Breaker's Responsibility:               │                        │
│  │ 1. Fix immediately (preferred)          │                        │
│  │ 2. Revert if can't fix in 30 min        │                        │
│  │ 3. All other work pauses until fixed    │                        │
│  └─────────────────────────────────────────┘                        │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Build Break Rules

| Rule | Rationale |
|------|-----------|
| Breaker fixes or reverts | Responsibility stays with cause |
| Fix in 30 minutes or revert | Don't leave team blocked |
| No commits during red build | Prevents compounding problems |
| Build cop has authority | Someone empowered to enforce |

## Framework: Integration Frequency

| Strategy | When to Use | Risk Level |
|----------|-------------|------------|
| **Continuous** | Every commit integrates | Low (problems found fast) |
| **Daily** | Integrate once per day | Medium (some delay) |
| **Feature-based** | Integrate when feature complete | High (big bang problems) |
| **Sprint-based** | Integrate at sprint end | Very high (not recommended) |

**Recommendation:** Continuous integration with daily builds minimum.

## Framework: Automated Test Gates

| Test Type | When Run | Failure Blocks |
|-----------|----------|----------------|
| **Compile** | Every commit | Merge |
| **Unit Tests** | Every commit | Merge |
| **Integration Tests** | Daily | Next day's QA |
| **Smoke Tests** | Daily | Release |
| **Full Regression** | Weekly/milestone | Release |
| **Performance Tests** | Weekly | Release (if degraded) |

### Test Coverage Targets

| Component | Target Coverage | Current |
|-----------|-----------------|---------|
| Core gameplay | 70%+ | |
| Economy/transactions | 90%+ | |
| Save/load | 80%+ | |
| UI flows | 50%+ | |
| Networking | 70%+ | |

## Framework: Build Stability Metrics

| Metric | Target | Current | Trend |
|--------|--------|---------|-------|
| Build success rate | >95% | | |
| Average time to fix break | <1 hour | | |
| Build time (CI) | <15 min | | |
| Build time (full) | <30 min | | |
| Days since last broken build | 7+ | | |

## Checklist

- [ ] CI pipeline configured
- [ ] Build break alerts configured
- [ ] Build break protocol documented
- [ ] Test gates defined
- [ ] Build cop role assigned (rotating)
- [ ] Metrics dashboard available
- [ ] Team trained on protocol

## Tasks

1. **Set up CI pipeline** if not already in place
2. **Configure automated alerts** for build breaks
3. **Define your test gates** and coverage targets
4. **Establish build cop rotation**
5. **Create build health dashboard**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.8 Config vs. Code Separation

## Why It Matters

Every decision baked into code requires a client update to change—days or weeks of build, QA, submission, and rollout. Config-driven values can change in minutes. Knowing what to externalize to config vs. what to keep in code determines your operational agility post-launch.

## Framework: Config vs. Code Decision Matrix

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CONFIG vs. CODE DECISION MATRIX                  │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                     CHANGE FREQUENCY                                │
│              Low                          High                      │
│         ┌─────────────────────────────────────────┐                 │
│         │                    │                    │                 │
│    Low  │     CODE           │    REMOTE CONFIG  │  IMPACT         │
│         │                    │                   │                  │
│         │  Core algorithms   │  Feature flags    │                 │
│         │  Architecture      │  UI text          │                 │
│         │  Engine systems    │  Simple toggles   │                 │
│         │                    │                   │                 │
│         ├────────────────────┼───────────────────┤                 │
│         │                    │                   │                 │
│    High │   CODE + REVIEW    │  CONFIG + GUARDRAILS               │
│         │                    │                   │                 │
│         │  Balance formulas  │  Economy values   │                 │
│         │  Progression       │  Event configs    │                 │
│         │  Security          │  Offer prices     │                 │
│         │                    │                   │                 │
│         └─────────────────────────────────────────┘                 │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: What to Config vs. Code

### Always Code (Never Config)

| Category | Examples | Reason |
|----------|----------|--------|
| Security | Authentication, encryption | Security risk if externalized |
| Core mechanics | Physics, collision | Stability/exploit risk |
| Platform integration | Store APIs, social | SDK requirements |
| Data structures | Save format, database schema | Migration complexity |

### Always Config (Remote Preferred)

| Category | Examples | Reason |
|----------|----------|--------|
| Economy values | Prices, rewards, drop rates | Constant tuning needed |
| Event definitions | Timing, rewards, structure | Operational flexibility |
| Feature flags | Enable/disable features | Quick response to issues |
| UI text | Strings, messages | Localization, updates |
| Offers | Contents, pricing, display | Real-time optimization |

### Context-Dependent

| Category | Code When... | Config When... |
|----------|--------------|----------------|
| Balance values | Formula/algorithm changes | Number tuning only |
| Difficulty | Curve structure changes | Value adjustments |
| Matchmaking | Algorithm changes | Threshold tuning |
| Content | New mechanics needed | Variations of existing |

## Framework: Config Types Hierarchy

```
┌─────────────────────────────────────────────────────────────────────┐
│                    CONFIG HIERARCHY                                 │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  REMOTE CONFIG (Server-controlled)                            │  │
│  │  • Changes instantly without client update                    │  │
│  │  • Requires server infrastructure                             │  │
│  │  • Can segment by user/device/region                          │  │
│  │  • Examples: Feature flags, economy values, events            │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                           │                                         │
│                           ▼                                         │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  BUNDLED CONFIG (Client-side files)                           │  │
│  │  • Changes require client update                              │  │
│  │  • No server dependency                                       │  │
│  │  • Can be overridden by remote config                         │  │
│  │  • Examples: Default values, level layouts, localization      │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                           │                                         │
│                           ▼                                         │
│  ┌───────────────────────────────────────────────────────────────┐  │
│  │  HARDCODED (In code)                                          │  │
│  │  • Changes require code changes + client update               │  │
│  │  • Most stable, hardest to change                             │  │
│  │  • Examples: Core algorithms, security                        │  │
│  └───────────────────────────────────────────────────────────────┘  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Config Planning Template

For each game system, decide:

| System | Values | Remote Config? | Bundled Config? | Code? |
|--------|--------|---------------|-----------------|-------|
| **Economy** | | | | |
| Currency rewards | ✓ | | |
| IAP prices | ✓ | | |
| Drop rates | ✓ | | |
| **Gameplay** | | | | |
| Player stats | | ✓ | |
| Enemy stats | ✓ | | |
| Level layouts | | | ✓ |
| **Meta** | | | | |
| Event schedules | ✓ | | |
| Offer definitions | ✓ | | |
| Feature flags | ✓ | | |
| **UI** | | | | |
| Strings/text | | ✓ (+ remote for urgent) | |
| Tutorial steps | | ✓ | |

## Framework: Config Safety Guidelines

| Risk | Mitigation |
|------|------------|
| Bad config breaks game | Validation before deploy |
| Config exploited | Range limits, server validation |
| Config loss | Bundled fallback values |
| Wrong segment targeted | Staged rollout, preview |
| Can't rollback | Version history, one-click revert |

### Config Validation Checklist

| Check | Automated? |
|-------|------------|
| Schema validation (correct types) | Yes |
| Range validation (reasonable values) | Yes |
| Reference validation (IDs exist) | Yes |
| Consistency validation (A < B) | Yes |
| Business rules (price > 0) | Yes |
| Human review for critical changes | No (manual) |

## Checklist

- [ ] Each system categorized (config vs. code)
- [ ] Remote config infrastructure selected
- [ ] Bundled config format defined
- [ ] Fallback behavior documented
- [ ] Validation rules implemented
- [ ] Change process documented
- [ ] Team trained on what can change remotely

## Tasks

1. **Audit all game values** — categorize each
2. **Select remote config solution** (Firebase, custom, etc.)
3. **Design config schema** for key systems
4. **Implement validation layer**
5. **Document what's remotely tunable** for live ops team

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.9 Remote Config Management

## Why It Matters

Remote config is powerful but dangerous. A typo can crash the game for millions. A bad value can destroy the economy. A misconfigured segment can give free items to everyone. Safe deployment, rollback capability, and A/B test integration turn remote config from a liability into a competitive advantage.

## Framework: Remote Config Deployment Pipeline

```
┌─────────────────────────────────────────────────────────────────────┐
│                    REMOTE CONFIG DEPLOYMENT                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  AUTHOR           REVIEW           STAGE            DEPLOY          │
│                                                                     │
│  ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐          │
│  │ Create/ │───►│ Peer    │───►│ Test in │───►│ Staged  │          │
│  │ Edit    │    │ Review  │    │ Staging │    │ Rollout │          │
│  │ Config  │    │         │    │         │    │         │          │
│  └─────────┘    └─────────┘    └─────────┘    └─────────┘          │
│       │              │              │              │                │
│       ▼              ▼              ▼              ▼                │
│  ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐          │
│  │ Schema  │    │ Business│    │ QA      │    │ Monitor │          │
│  │ Valid.  │    │ Review  │    │ Sign-off│    │ Metrics │          │
│  └─────────┘    └─────────┘    └─────────┘    └─────────┘          │
│                                                                     │
│  Rollback available at any stage                                    │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Staged Rollout Process

| Stage | Audience | Duration | Success Criteria |
|-------|----------|----------|------------------|
| **1. Internal** | Team only | 1 hour | No crashes, values correct |
| **2. Canary** | 1% of users | 1-4 hours | No metric anomalies |
| **3. Limited** | 10% of users | 4-24 hours | No negative impact |
| **4. Broad** | 50% of users | 24 hours | Metrics stable |
| **5. Full** | 100% of users | Ongoing | Monitoring continues |

### Rollout Decision Points

| Metric | Acceptable Range | Action if Outside |
|--------|------------------|-------------------|
| Crash rate | < 1% increase | Pause/rollback |
| Error rate | < 5% increase | Pause/rollback |
| Revenue | > 90% of baseline | Pause/investigate |
| Session length | > 90% of baseline | Pause/investigate |

## Framework: Rollback Protocol

```
┌─────────────────────────────────────────────────────────────────────┐
│                    ROLLBACK DECISION TREE                           │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│                    ISSUE DETECTED                                   │
│                         │                                           │
│            ┌────────────┴────────────┐                              │
│            ▼                         ▼                              │
│     ┌──────────────┐         ┌──────────────┐                       │
│     │ Game-breaking│         │ Non-critical │                       │
│     │ (Crash/Econ) │         │ (Minor bug)  │                       │
│     └──────┬───────┘         └──────┬───────┘                       │
│            │                        │                               │
│            ▼                        ▼                               │
│     ┌──────────────┐         ┌──────────────┐                       │
│     │ IMMEDIATE    │         │ FIX FORWARD  │                       │
│     │ ROLLBACK     │         │ (New config) │                       │
│     └──────────────┘         └──────────────┘                       │
│                                                                     │
│  Rollback Execution:                                                │
│  1. One-click revert to last known good config                      │
│  2. Verify revert successful (metrics stabilize)                    │
│  3. Notify team and document incident                               │
│  4. Post-mortem within 24 hours                                     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Rollback Readiness Checklist

| Requirement | Status |
|-------------|--------|
| Previous config version stored | ☐ |
| One-click rollback available | ☐ |
| Rollback tested recently | ☐ |
| Rollback doesn't require client update | ☐ |
| Team knows how to rollback | ☐ |
| Rollback alerting configured | ☐ |

## Framework: A/B Test Integration

### Config-Based A/B Tests

| Element | Control | Variant A | Variant B |
|---------|---------|-----------|-----------|
| Config key | `reward_amount` | `reward_amount` | `reward_amount` |
| Value | 100 | 150 | 200 |
| Segment | 33% random | 33% random | 33% random |
| Duration | 7 days | 7 days | 7 days |
| Primary metric | D7 retention | D7 retention | D7 retention |

### A/B Test Config Checklist

| Requirement | Verified |
|-------------|----------|
| Segments properly randomized | ☐ |
| Assignment is sticky (user stays in same group) | ☐ |
| Test can be stopped early if harmful | ☐ |
| Results tracked with proper attribution | ☐ |
| Statistical significance calculated | ☐ |

## Framework: Config Change Request Template

```
CONFIG CHANGE REQUEST

Requester: _______________
Date: _______________
Priority: Routine / Urgent / Emergency

Config Key: _______________
Current Value: _______________
New Value: _______________

Reason for Change:
_______________________________________________________________________________

Expected Impact:
_______________________________________________________________________________

Rollback Plan:
_______________________________________________________________________________

Testing Completed: Yes / No
If yes, describe: _______________

Approvers Required: [ ] Economy [ ] Design [ ] Engineering [ ] Producer
```

## Framework: Config Governance

| Change Type | Approval Required | Staged Rollout |
|-------------|-------------------|----------------|
| Feature flag (enable) | Product + Engineering | Yes |
| Feature flag (disable) | Engineering (if emergency) | Optional |
| Economy values | Economy + Product | Yes |
| Event config | Live Ops + QA | Yes |
| Emergency fix | On-call + Document later | Optional |
| A/B test start | Product + Analytics | Yes |
| A/B test stop | Product | No |

## Checklist

- [ ] Config management tool selected
- [ ] Staged rollout process defined
- [ ] Rollback capability tested
- [ ] A/B test integration working
- [ ] Governance/approval process documented
- [ ] Change request workflow in place
- [ ] Team trained on deployment process

## Tasks

1. **Select config management tool** (or build)
2. **Implement staged rollout** capability
3. **Test rollback** end-to-end
4. **Create change request template**
5. **Document approval matrix**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.10 QA for Live Content

## Why It Matters

Live content QA is different from feature QA. The timeline is compressed (days not weeks), the content is often config-based (different bug types), and the stakes are immediate (broken event = lost revenue). A dedicated process ensures live content ships reliably without slowing down velocity.

## Framework: Live Content QA Pipeline

```
┌─────────────────────────────────────────────────────────────────────┐
│                    LIVE CONTENT QA PIPELINE                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  Day -5        Day -3         Day -1        Day 0         Day +1   │
│                                                                     │
│  ┌─────────┐  ┌─────────┐   ┌─────────┐   ┌─────────┐  ┌─────────┐ │
│  │ Content │  │ Deploy  │   │ Full QA │   │ Go Live │  │ Monitor │ │
│  │ Created │─►│ to      │──►│ Pass    │──►│         │─►│ & Fix   │ │
│  │         │  │ Staging │   │         │   │         │  │         │ │
│  └─────────┘  └─────────┘   └─────────┘   └─────────┘  └─────────┘ │
│       │            │             │             │             │      │
│       ▼            ▼             ▼             ▼             ▼      │
│  ┌─────────┐  ┌─────────┐   ┌─────────┐   ┌─────────┐  ┌─────────┐ │
│  │ Design  │  │ Smoke   │   │ QA      │   │ Live    │  │ Issue   │ │
│  │ Review  │  │ Test    │   │ Sign-off│   │ Check   │  │ Triage  │ │
│  └─────────┘  └─────────┘   └─────────┘   └─────────┘  └─────────┘ │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Event QA Test Matrix

| Test Category | Test Cases | Priority |
|---------------|------------|----------|
| **Start/End** | Event starts at correct time | Critical |
| | Event ends at correct time | Critical |
| | Timezone handling correct | Critical |
| | Grace period works | High |
| **Mechanics** | Core event mechanic functions | Critical |
| | Progression tracks correctly | Critical |
| | Difficulty appropriate | High |
| | Edge cases (max score, etc.) | Medium |
| **Rewards** | Correct rewards granted | Critical |
| | Rewards granted at right time | Critical |
| | Leaderboard rewards correct | High |
| | No duplicate rewards | Critical |
| **Display** | UI shows correct information | High |
| | Localization correct | High |
| | Art assets correct | High |
| | Timer displays accurate | High |
| **Integration** | Event with other features | Medium |
| | Save/load during event | High |
| | Session resume | High |

### Event QA Checklist Template

```
EVENT: _______________
QA: _______________
Date: _______________

PRE-LAUNCH VERIFICATION
[ ] Event config deployed to staging
[ ] Event appears in game at scheduled time
[ ] Event does not appear before scheduled time
[ ] All UI text correct (all languages)
[ ] All art assets correct

FUNCTIONAL TESTING
[ ] Core mechanic works
[ ] Scoring/progress tracks correctly
[ ] All rewards granted correctly
[ ] Leaderboard functions (if applicable)
[ ] Edge cases tested (see matrix)

TIMING TESTS
[ ] Start time verified (test in multiple timezones)
[ ] End time verified
[ ] Time display accurate during event
[ ] Post-event behavior correct

INTEGRATION TESTS
[ ] Save during event, load after
[ ] Session interrupt and resume
[ ] Event + other features (store, social, etc.)

SIGN-OFF
[ ] QA APPROVED / NOT APPROVED
Notes: _______________
```

## Framework: Offer QA Checklist

| Test | Expected | Actual | Pass? |
|------|----------|--------|-------|
| **Display** | | | |
| Correct price shown | | | |
| Correct contents shown | | | |
| Art matches contents | | | |
| Localization correct | | | |
| **Purchase Flow** | | | |
| Purchase button works | | | |
| Store flow completes | | | |
| Receipt processed | | | |
| Contents granted | | | |
| Analytics tracked | | | |
| **Edge Cases** | | | |
| Purchase limit enforced | | | |
| Already-owned handling | | | |
| Network interrupt | | | |
| Refund scenario | | | |

## Framework: Config Change QA

### Balance/Value Change Testing

| Aspect | Test |
|--------|------|
| **Direct Effect** | Changed value works as expected |
| **Downstream** | Dependent systems still work |
| **Economy** | No unintended currency generation |
| **Exploits** | Change doesn't enable exploits |
| **Performance** | Change doesn't affect performance |

### Config QA Checklist

```
CONFIG CHANGE: _______________
QA: _______________

[ ] New value applied correctly
[ ] Old value no longer active
[ ] Direct functionality verified
[ ] Related systems checked
[ ] No economy exploits possible
[ ] Rollback tested
[ ] Sign-off granted
```

## Framework: Staging Environment Requirements

| Requirement | Details |
|-------------|---------|
| **Parity** | Mirrors production as closely as possible |
| **Data** | Has realistic test data |
| **Time manipulation** | Can set server time for date testing |
| **Isolation** | Changes don't affect production |
| **Reset capability** | Can restore to clean state |
| **Access** | QA can deploy and configure |

## Framework: Live Content Bug Severity

| Severity | Definition | Examples | Response |
|----------|------------|----------|----------|
| **S1** | Cannot ship | Rewards wrong, crash, exploit | Fix required |
| **S2** | Major issue | UI broken, text wrong | Fix preferred |
| **S3** | Minor issue | Visual glitch, typo | Fix if time |
| **S4** | Polish | Slight misalignment | Defer |

## Checklist

- [ ] Live content QA pipeline defined
- [ ] Test matrices created per content type
- [ ] Staging environment ready
- [ ] QA sign-off process documented
- [ ] Bug severity matrix defined
- [ ] Timeline requirements agreed (how much lead time)

## Tasks

1. **Create test matrix** for your primary content types
2. **Set up staging environment** with time manipulation
3. **Define minimum QA timeline** per content type
4. **Train QA team** on live content specifics
5. **Create templates** for recurring content types

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.11 Bug Triage Framework

## Why It Matters

Not all bugs are equal—a crash in the tutorial is worse than a visual glitch in an optional menu. Without a consistent triage framework, teams waste time on low-impact bugs while high-impact issues wait. Live games need triage calibrated for revenue impact, not just technical severity.

## Framework: Severity × Priority Matrix

```
┌─────────────────────────────────────────────────────────────────────┐
│                    BUG SEVERITY × PRIORITY                          │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  SEVERITY (Technical Impact)                                        │
│                                                                     │
│  S1-Critical   Game crashes, data loss, security breach            │
│  S2-Major      Feature broken, significant UX issue                │
│  S3-Moderate   Feature impaired but workaround exists              │
│  S4-Minor      Cosmetic issue, minor inconvenience                 │
│                                                                     │
│  PRIORITY (Business Impact)                                         │
│                                                                     │
│  P1-Urgent     Blocking release, losing revenue NOW                │
│  P2-High       Significant player impact, fix this sprint          │
│  P3-Medium     Should fix, but not blocking                        │
│  P4-Low        Nice to fix, address when convenient                │
│                                                                     │
│               P1        P2        P3        P4                      │
│          ┌─────────┬─────────┬─────────┬─────────┐                  │
│     S1   │   FIX   │   FIX   │   FIX   │  PLAN   │                  │
│          │   NOW   │  TODAY  │  SPRINT │         │                  │
│          ├─────────┼─────────┼─────────┼─────────┤                  │
│     S2   │   FIX   │   FIX   │  PLAN   │ BACKLOG │                  │
│          │  TODAY  │  SPRINT │         │         │                  │
│          ├─────────┼─────────┼─────────┼─────────┤                  │
│     S3   │   FIX   │  PLAN   │ BACKLOG │ BACKLOG │                  │
│          │  SPRINT │         │         │         │                  │
│          ├─────────┼─────────┼─────────┼─────────┤                  │
│     S4   │  PLAN   │ BACKLOG │ BACKLOG │  WONT   │                  │
│          │         │         │         │   FIX   │                  │
│          └─────────┴─────────┴─────────┴─────────┘                  │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Live Game Bug Severity Definitions

### S1 - Critical

| Criteria | Examples |
|----------|----------|
| Game crashes for >1% of users | Startup crash on specific device |
| Data loss or corruption | Save file corrupted |
| Security vulnerability | Exploit allowing free purchases |
| Economy exploit | Infinite currency glitch |
| Progression blocker | Cannot continue story |
| IAP not delivering | Purchase succeeds, no items |

### S2 - Major

| Criteria | Examples |
|----------|----------|
| Major feature non-functional | Multiplayer won't connect |
| Significant revenue impact | Offers not appearing |
| Frequent annoyance | Regular soft-lock requiring restart |
| Certification blocker | Platform requirement violated |
| Major UX issue | Tutorial impossible to complete |

### S3 - Moderate

| Criteria | Examples |
|----------|----------|
| Feature impaired | Leaderboard loads slowly |
| Workaround available | Alternative path to goal |
| Intermittent issue | Sometimes happens |
| Moderate UX issue | Confusing but completable |
| Localization error | Wrong language occasionally |

### S4 - Minor

| Criteria | Examples |
|----------|----------|
| Cosmetic issues | Visual glitch, misalignment |
| Rare occurrence | Edge case scenario |
| Minimal impact | Slightly wrong color |
| Polish items | Animation could be smoother |

## Framework: Priority Factors for Live Games

| Factor | Increases Priority | Decreases Priority |
|--------|-------------------|-------------------|
| **Revenue impact** | Affects purchases, monetization | Non-monetized area |
| **User reach** | All users affected | Rare edge case |
| **Timing** | During major event/campaign | Non-critical period |
| **Visibility** | Early game, common path | Late game, optional |
| **PR/reviews** | Review-impacting | Not visible externally |
| **Competitive** | Players comparing to competitor | Non-competitive feature |

### Priority Decision Questions

1. Is this causing us to lose revenue right now? → P1
2. Could this affect app store ratings? → P1-P2
3. Is this blocking a scheduled release? → P1
4. Is this affecting an active event? → P1-P2
5. How many users are impacted? → Scale accordingly

## Framework: Bug Triage Meeting Structure

| Element | Duration | Purpose |
|---------|----------|---------|
| **New bugs review** | 15 min | Classify incoming bugs |
| **P1/P2 status** | 10 min | Progress on urgent issues |
| **Sprint bug review** | 10 min | On track for sprint fixes? |
| **Old bugs cleanup** | 5 min | Close/defer stale bugs |

### Triage Roles

| Role | Responsibility |
|------|----------------|
| **QA Lead** | Presents new bugs, provides context |
| **Engineering Lead** | Estimates effort, identifies complexity |
| **Producer** | Prioritizes based on business impact |
| **Product** | Provides player impact perspective |

## Framework: Bug Resolution Targets

| Classification | Resolution Target | Escalate If |
|----------------|-------------------|-------------|
| S1P1 | < 4 hours | Not fixed in 2 hours |
| S1P2 / S2P1 | < 24 hours | Not fixed in 8 hours |
| S2P2 | This sprint | Not assigned in 2 days |
| S3P2 / S2P3 | Next sprint | Aging > 30 days |
| Other | Backlog | Aging > 90 days |

## Framework: Bug Database Hygiene

| Task | Frequency | Owner |
|------|-----------|-------|
| Triage new bugs | Daily | QA Lead |
| Review P1/P2 progress | Daily | Engineering Lead |
| Sprint bug planning | Per sprint | Team |
| Old bug review (>30 days) | Weekly | QA |
| Database cleanup (close stale) | Monthly | QA |

## Checklist

- [ ] Severity definitions documented
- [ ] Priority factors listed
- [ ] Severity × Priority matrix agreed
- [ ] Triage meeting cadence set
- [ ] Resolution targets defined
- [ ] Roles assigned
- [ ] Database hygiene process in place

## Tasks

1. **Customize severity definitions** for your game
2. **Create priority rubric** with revenue factors
3. **Set up triage meeting** rhythm
4. **Define resolution targets** and escalation
5. **Train team** on consistent classification

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.12 Hotfix Pipeline

## Why It Matters

When a critical bug hits production, the normal release process (days to weeks) is too slow. Lost revenue, angry players, and potential PR disasters demand fast action. A hotfix pipeline enables emergency client updates in hours instead of days while maintaining enough process to avoid making things worse.

## Framework: Hotfix vs. Regular Release

```
┌─────────────────────────────────────────────────────────────────────┐
│              REGULAR RELEASE vs. HOTFIX                             │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  REGULAR RELEASE                    HOTFIX                          │
│  (Days/Weeks)                       (Hours)                         │
│                                                                     │
│  ┌──────────────────────┐          ┌──────────────────────┐        │
│  │ Full feature work    │          │ Critical fix ONLY    │        │
│  │ Complete QA pass     │          │ Targeted testing     │        │
│  │ Full regression      │          │ Smoke test + fix area│        │
│  │ Platform review      │          │ Expedited review     │        │
│  │ Staged rollout       │          │ Fast rollout         │        │
│  │ Full docs            │          │ Minimal docs         │        │
│  └──────────────────────┘          └──────────────────────┘        │
│                                                                     │
│  Use when:                          Use when:                       │
│  • Normal development               • S1/P1 bug in production       │
│  • Planned features                 • Revenue loss occurring        │
│  • Non-urgent fixes                 • Security vulnerability        │
│  • Content updates                  • Certification failure         │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Hotfix Criteria

### Hotfix IS Appropriate

| Situation | Example |
|-----------|---------|
| Crash affecting >1% of users | Startup crash on popular device |
| Active revenue loss | Purchase flow broken |
| Security vulnerability | Exploit discovered |
| Event-breaking bug | Live event non-functional |
| Certification failure | Just submitted, must fix fast |
| Data corruption | Player progress being lost |

### Hotfix IS NOT Appropriate

| Situation | Better Approach |
|-----------|-----------------|
| Minor visual bug | Next regular release |
| Feature that can wait | Next regular release |
| Low-impact issue | Config fix if possible |
| Edge case | Document, next release |
| "Nice to have" fix | Next regular release |

## Framework: Hotfix Pipeline Steps

```
┌─────────────────────────────────────────────────────────────────────┐
│                    HOTFIX PIPELINE                                  │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  TRIGGER          FIX            TEST           DEPLOY              │
│  (30 min)         (1-4 hrs)      (1-2 hrs)      (1-24 hrs)         │
│                                                                     │
│  ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐          │
│  │ Issue   │───►│ Develop │───►│ Smoke + │───►│ Submit/ │          │
│  │ Verified│    │ Fix     │    │ Targeted│    │ Release │          │
│  └─────────┘    └─────────┘    └─────────┘    └─────────┘          │
│       │              │              │              │                │
│       ▼              ▼              ▼              ▼                │
│  ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐          │
│  │Approve  │    │ Code    │    │ QA      │    │ Monitor │          │
│  │Hotfix   │    │ Review  │    │ Sign-off│    │ Post-   │          │
│  │         │    │ (Quick) │    │         │    │ Release │          │
│  └─────────┘    └─────────┘    └─────────┘    └─────────┘          │
│                                                                     │
│  Total Target Time: 4-8 hours (platform submission may add time)   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

### Step Details

| Step | Duration | Owner | Actions |
|------|----------|-------|---------|
| **1. Trigger** | <30 min | On-call | Verify issue, assess severity, approve hotfix |
| **2. Fix** | 1-4 hrs | Engineer | Develop minimal fix, code review |
| **3. Test** | 1-2 hrs | QA | Smoke test + targeted fix testing |
| **4. Deploy** | 1-24 hrs | Release | Submit to stores, staged rollout |
| **5. Monitor** | 24 hrs | On-call | Verify fix working, no new issues |

## Framework: Hotfix Approval Matrix

| Approver | When Required |
|----------|---------------|
| Engineering Lead | Always (technical approval) |
| Producer | Always (business approval) |
| QA Lead | Always (quality approval) |
| Studio Head/Director | Major incidents, high-risk fixes |

## Framework: Hotfix Testing Requirements

### Minimum Testing (Always Required)

| Test | Purpose |
|------|---------|
| Fix verification | Bug actually fixed |
| Smoke test | Game launches, core loop works |
| Regression on affected area | Didn't break related features |
| Multi-platform (if applicable) | Works on all shipping platforms |

### Skipped in Hotfix (Document Risk)

| Test | Risk of Skipping |
|------|------------------|
| Full regression | May miss unrelated breakage |
| Edge case testing | May miss related bugs |
| Performance testing | May impact performance |
| Localization testing | May break non-English |

## Framework: Platform Submission Expediting

| Platform | Normal Review | Expedited Review | How to Request |
|----------|---------------|------------------|----------------|
| **iOS** | 1-3 days | 24 hours | Request expedited review in App Store Connect |
| **Google Play** | Hours-1 day | Similar | Usually fast already |
| **Steam** | Instant (PC) | Instant | Self-publish |
| **Console** | 3-7 days | 1-3 days | Contact platform rep, explain emergency |

### Expedited Review Request Template

```
Subject: Emergency Hotfix - [Game Name] - Critical Issue

Issue: [Brief description of critical issue]
Impact: [Number of users affected, revenue impact]
Fix: [Brief description of fix]
Testing: [Summary of testing completed]

We request an expedited review for this critical hotfix.
Contact: [Your phone number]
```

## Framework: Post-Hotfix Actions

| Action | Timing | Owner |
|--------|--------|-------|
| Monitor fix effectiveness | 24-48 hours | On-call |
| Post-mortem meeting | Within 72 hours | Team |
| Document root cause | Within 1 week | Engineering |
| Preventive measures identified | Within 1 week | Team |
| Process improvements implemented | Within 2 weeks | Process owner |

## Checklist

- [ ] Hotfix criteria defined
- [ ] Approval matrix documented
- [ ] Pipeline steps and timings agreed
- [ ] Testing requirements documented
- [ ] Platform contacts available
- [ ] Post-hotfix process defined
- [ ] Team trained on hotfix process

## Tasks

1. **Document hotfix criteria** specific to your game
2. **Create approval contact list** (phone numbers, not just email)
3. **Test the pipeline** with a simulated hotfix
4. **Establish platform relationships** for expedited review
5. **Create post-mortem template**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.13 A/B Test Implementation Standards

## Why It Matters

A/B tests promise data-driven decisions, but poor implementation leads to bad data and worse decisions. Overlapping tests pollute results. Inconsistent tracking makes comparison impossible. Lack of statistical rigor leads to false conclusions. Standards ensure your tests actually tell you something true.

## Framework: A/B Test Lifecycle

```
┌─────────────────────────────────────────────────────────────────────┐
│                    A/B TEST LIFECYCLE                               │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  PLAN            IMPLEMENT        RUN             ANALYZE           │
│  (1-2 days)      (1-3 days)      (7-30 days)     (1-2 days)        │
│                                                                     │
│  ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐          │
│  │Hypothesis│───►│Setup &  │───►│Monitor &│───►│Conclude │          │
│  │& Design │    │Validate │    │Wait     │    │& Apply  │          │
│  └─────────┘    └─────────┘    └─────────┘    └─────────┘          │
│       │              │              │              │                │
│       ▼              ▼              ▼              ▼                │
│  ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐          │
│  │ Define  │    │ Config  │    │ DON'T   │    │Document │          │
│  │ metrics │    │ tracking│    │ PEEK    │    │learnings│          │
│  │ sample  │    │ verify  │    │ (mostly)│    │         │          │
│  └─────────┘    └─────────┘    └─────────┘    └─────────┘          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Test Design Standards

### Hypothesis Format

**Template:**
```
If we [make change], 
then [primary metric] will [increase/decrease] 
because [reasoning].
```

**Example:**
```
If we reduce first-purchase price from $4.99 to $2.99,
then conversion rate will increase by 50%+
because price is the primary barrier for first purchase.
```

### Test Documentation Template

| Field | Content |
|-------|---------|
| **Test Name** | Clear, descriptive name |
| **Hypothesis** | Using template above |
| **Primary Metric** | Single metric for decision |
| **Secondary Metrics** | Supporting metrics (max 3) |
| **Guardrail Metrics** | Metrics that must not degrade |
| **Variants** | Control + 1-3 treatments |
| **Sample Size** | Calculated minimum per variant |
| **Duration** | Minimum run time |
| **Success Criteria** | What constitutes a win |

## Framework: Sample Size & Duration

### Sample Size Calculation Factors

| Factor | Impact on Sample Size |
|--------|----------------------|
| Baseline conversion rate | Lower baseline = larger sample needed |
| Minimum detectable effect | Smaller effect = larger sample needed |
| Statistical significance (typically 95%) | Higher confidence = larger sample needed |
| Statistical power (typically 80%) | Higher power = larger sample needed |

### Quick Reference Sample Sizes

| Baseline Rate | 10% Lift | 20% Lift | 50% Lift |
|---------------|----------|----------|----------|
| 1% | 150,000 | 40,000 | 7,000 |
| 5% | 30,000 | 8,000 | 1,500 |
| 10% | 15,000 | 4,000 | 700 |
| 20% | 7,000 | 2,000 | 400 |

*Per variant, for 95% confidence / 80% power*

### Minimum Duration Rules

| Rule | Rationale |
|------|-----------|
| At least 1 full week | Capture day-of-week variation |
| At least 2 full cycles | Capture user behavior patterns |
| Until sample size reached | Statistical validity |
| No peeking before minimum | Avoid false positives |

## Framework: Tracking Implementation

### Required Events per Test

| Event | Data Fields | When Fired |
|-------|-------------|------------|
| test_enrolled | user_id, test_id, variant, timestamp | On first exposure |
| test_exposure | user_id, test_id, variant, context | Each exposure |
| [primary_metric] | user_id, value, test_id, variant | When metric occurs |
| [secondary_metrics] | user_id, value, test_id, variant | When metrics occur |

### Tracking Validation Checklist

| Check | Method |
|-------|--------|
| Events firing correctly | QA verification in staging |
| Correct variant assignment | Check user distribution |
| Assignment is sticky | Same user = same variant |
| No cross-contamination | Variants isolated |
| Data reaching warehouse | End-to-end validation |

## Framework: Test Isolation Standards

### Avoiding Test Interaction

| Rule | Implementation |
|------|----------------|
| One test per user journey | User in onboarding test excluded from monetization test |
| No overlapping metrics | Tests measuring same metric cannot run simultaneously |
| Holdout groups | Maintain global holdout for cumulative measurement |
| Test layering | Use orthogonal assignment for independent tests |

### Test Interaction Matrix

Before starting a test, check:

| New Test Area | Can Run With | Cannot Run With |
|---------------|--------------|-----------------|
| Onboarding | Monetization, Meta | Other onboarding |
| Monetization | Onboarding, Gameplay | Other monetization |
| Core Gameplay | Onboarding, Monetization | Other core gameplay |

## Framework: Statistical Rigor Checklist

### Before Test

- [ ] Hypothesis documented
- [ ] Primary metric defined (single metric)
- [ ] Sample size calculated
- [ ] Minimum duration set
- [ ] Tracking validated
- [ ] No conflicting tests running

### During Test

- [ ] DON'T PEEK at results (mostly)
- [ ] Monitor for technical issues only
- [ ] Emergency stop criteria defined
- [ ] No mid-test changes to variants

### After Test

- [ ] Statistical significance reached?
- [ ] Practical significance assessed?
- [ ] Secondary metrics reviewed?
- [ ] Guardrail metrics checked?
- [ ] Decision documented?
- [ ] Learnings captured?

## Framework: Decision Framework

| Outcome | Criteria | Action |
|---------|----------|--------|
| **Winner** | p < 0.05, practical effect size, no guardrail issues | Ship winning variant |
| **No Winner** | p > 0.05, within noise | Keep control, document learning |
| **Mixed** | Primary positive, guardrail negative | Further investigation |
| **Loser** | Control wins significantly | Keep control, document learning |
| **Inconclusive** | Sample size not reached | Extend or redesign test |

## Checklist

- [ ] Test design template created
- [ ] Sample size calculator available
- [ ] Tracking standards documented
- [ ] Isolation rules defined
- [ ] Statistical rigor checklist in use
- [ ] Decision framework agreed
- [ ] Learning repository established

## Tasks

1. **Create test design template** for your team
2. **Set up sample size calculator** (or use existing tool)
3. **Validate tracking infrastructure** end-to-end
4. **Document active tests** and isolation rules
5. **Establish learning repository** for past tests

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.14 Data Logging Standards

## Why It Matters

"We should have tracked that" is the saddest phrase in analytics. By the time you realize you need data, it's too late—the players are gone, the event is over, the decision must be made. Comprehensive logging standards ensure you capture what you need before you know you need it.

## Framework: Event Taxonomy

```
┌─────────────────────────────────────────────────────────────────────┐
│                    EVENT TAXONOMY STRUCTURE                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  CATEGORY          SUBCATEGORY          EVENT                       │
│                                                                     │
│  session           ─┬─ lifecycle        session_start               │
│                     │                   session_end                 │
│                     └─ quality          session_crash               │
│                                                                     │
│  progression       ─┬─ level            level_start                 │
│                     │                   level_complete              │
│                     │                   level_fail                  │
│                     └─ milestone        tutorial_complete           │
│                                                                     │
│  economy           ─┬─ earn             currency_earned             │
│                     │                   item_acquired               │
│                     └─ spend            currency_spent              │
│                                         item_consumed               │
│                                                                     │
│  monetization      ─┬─ impression       offer_shown                 │
│                     │                   store_opened                │
│                     └─ transaction      purchase_start              │
│                                         purchase_complete           │
│                                         purchase_fail               │
│                                                                     │
│  engagement        ─┬─ feature          feature_used                │
│                     │                   menu_opened                 │
│                     └─ social           friend_added                │
│                                         share_completed             │
│                                                                     │
│  technical         ─┬─ performance      fps_sample                  │
│                     │                   load_time                   │
│                     └─ error            error_occurred              │
│                                         crash_detected              │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Event Schema Standards

### Universal Properties (Every Event)

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| event_name | string | Event identifier | "purchase_complete" |
| timestamp | datetime | When event occurred | "2024-01-15T14:30:00Z" |
| user_id | string | Unique user identifier | "u_abc123" |
| session_id | string | Current session | "s_xyz789" |
| client_version | string | App version | "1.2.3" |
| platform | string | Device platform | "iOS" / "Android" |
| device_model | string | Device type | "iPhone 14" |
| country | string | User country | "US" |
| ab_tests | object | Active test variants | {"test_1": "A"} |

### Event-Specific Properties

| Event | Required Properties | Optional Properties |
|-------|---------------------|---------------------|
| level_complete | level_id, time_spent, score | stars, deaths, retries |
| purchase_complete | product_id, price, currency | offer_id, source |
| currency_earned | currency_type, amount, source | level_id, feature |
| currency_spent | currency_type, amount, sink | item_id, quantity |
| session_start | install_date, days_since_install | referrer |

## Framework: Funnel Event Requirements

### User Acquisition Funnel

| Stage | Event | Key Properties |
|-------|-------|----------------|
| Install | app_install | source, campaign, creative |
| First Launch | session_start (first=true) | time_since_install |
| Tutorial Start | tutorial_start | - |
| Tutorial Complete | tutorial_complete | duration, skipped |
| First Action | first_[action] | - |
| First Session End | session_end (first=true) | duration |

### Monetization Funnel

| Stage | Event | Key Properties |
|-------|-------|----------------|
| Store View | store_opened | source, trigger |
| Product View | product_viewed | product_id, price |
| Purchase Start | purchase_start | product_id, price |
| Purchase Complete | purchase_complete | product_id, price, receipt |
| Purchase Fail | purchase_fail | product_id, error_code |

### Engagement Funnel (Per Feature)

| Stage | Event | Key Properties |
|-------|-------|----------------|
| Feature Visible | [feature]_shown | context |
| Feature Engaged | [feature]_started | - |
| Feature Completed | [feature]_completed | result, duration |
| Feature Repeated | [feature]_started (n>1) | attempt_number |

## Framework: Economy Tracking

### Currency Flow Events

| Event | Required Fields | Example |
|-------|-----------------|---------|
| currency_earned | currency_type, amount, source | "gems", 100, "level_reward" |
| currency_spent | currency_type, amount, sink | "gems", 50, "gacha_pull" |
| currency_converted | from_type, from_amount, to_type, to_amount | "gems", 100, "gold", 10000 |

### Inventory Events

| Event | Required Fields | Example |
|-------|-----------------|---------|
| item_acquired | item_id, quantity, source | "sword_01", 1, "purchase" |
| item_consumed | item_id, quantity, sink | "potion_hp", 1, "battle" |
| item_upgraded | item_id, from_level, to_level | "sword_01", 3, 4 |
| item_equipped | item_id, slot | "sword_01", "weapon" |

## Framework: Data Quality Checklist

### Implementation Validation

| Check | How to Verify |
|-------|---------------|
| Events fire when expected | QA walkthrough with logging enabled |
| All required properties present | Schema validation |
| Property types correct | Type checking |
| Values within expected ranges | Range validation |
| No duplicate events | Deduplication check |
| Events reach warehouse | End-to-end test |

### Ongoing Monitoring

| Metric | Alert Threshold |
|--------|-----------------|
| Event volume vs. baseline | ±30% deviation |
| Null property rate | >5% nulls in required field |
| Invalid value rate | >1% invalid values |
| Latency to warehouse | >1 hour delay |
| Schema violations | Any |

## Framework: Logging Level Definitions

| Level | When to Use | Volume Impact | Example |
|-------|-------------|---------------|---------|
| **Critical** | Every user, every time | Low | session_start, purchase_complete |
| **Standard** | Every occurrence | Medium | level_complete, currency_spent |
| **Detailed** | Sampling or debug | High | tap_location, fps_sample |
| **Debug** | Dev builds only | Very High | function_call, state_change |

## Framework: Documentation Requirements

### Event Catalog Entry

```
EVENT: purchase_complete

Description: Fires when a real-money purchase completes successfully

Category: monetization.transaction

Properties:
| Name | Type | Required | Description |
|------|------|----------|-------------|
| product_id | string | Yes | Store product identifier |
| price | float | Yes | Price charged |
| currency | string | Yes | Currency code (USD, EUR, etc.) |
| offer_id | string | No | If from special offer |
| source | string | No | Where purchase initiated |

Trigger: After receipt validation confirms success

Example:
{
  "event": "purchase_complete",
  "product_id": "gems_100",
  "price": 4.99,
  "currency": "USD",
  "offer_id": "welcome_bundle",
  "source": "store"
}
```

## Checklist

- [ ] Event taxonomy defined
- [ ] Universal properties standardized
- [ ] Key funnels instrumented
- [ ] Economy events complete
- [ ] Data quality monitoring in place
- [ ] Event catalog documented
- [ ] Team trained on logging standards

## Tasks

1. **Define your event taxonomy** using the structure above
2. **Create universal property standards** for your game
3. **Map key funnels** and required events
4. **Document economy flow** events
5. **Set up data quality monitoring**

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# 4A.15 Daily & Weekly Production Reviews

## Why It Matters

Without regular reviews, problems accumulate unseen. Small schedule slips compound into missed milestones. Emerging blockers become crises. Quality degrades gradually. Daily and weekly reviews create feedback loops that catch issues early and keep the team aligned.

## Framework: Review Cadence Structure

```
┌─────────────────────────────────────────────────────────────────────┐
│                    PRODUCTION REVIEW CADENCE                        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  DAILY                                                              │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ Stand-up (15 min)                                           │   │
│  │ • What did you complete?                                    │   │
│  │ • What will you complete today?                             │   │
│  │ • What's blocking you?                                      │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                                                                     │
│  WEEKLY                                                             │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ Production Review (30-60 min)                               │   │
│  │ • Sprint/milestone progress                                 │   │
│  │ • Risks and blockers                                        │   │
│  │ • Quality status                                            │   │
│  │ • Live metrics (if applicable)                              │   │
│  │ • Coming week priorities                                    │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                                                                     │
│  SPRINT/MILESTONE                                                   │
│  ┌─────────────────────────────────────────────────────────────┐   │
│  │ Sprint Review + Retrospective (1-2 hours)                   │   │
│  │ • Demo completed work                                       │   │
│  │ • Review metrics and goals                                  │   │
│  │ • Retrospective: What went well? What didn't?               │   │
│  │ • Plan improvements                                         │   │
│  └─────────────────────────────────────────────────────────────┘   │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

## Framework: Daily Stand-up Structure

### Format Options

| Format | Best For | Duration |
|--------|----------|----------|
| **Round-robin** | Small teams (<8), new teams | 15 min |
| **Walk-the-board** | Kanban teams, flow focus | 15 min |
| **Exception-based** | Experienced teams, large groups | 10 min |
| **Async** | Distributed teams, timezone spread | N/A |

### Stand-up Rules

| Rule | Rationale |
|------|-----------|
| Same time every day | Creates habit, maximizes attendance |
| 15 minutes max | Respects time, forces conciseness |
| Standing (if in-person) | Keeps it short |
| Blockers → Action | Don't just report, solve after |
| Updates only for team | Skip solo deep-dives |

### Stand-up Checklist

- [ ] Start on time (don't wait for latecomers)
- [ ] Follow chosen format
- [ ] Capture blockers explicitly
- [ ] Schedule follow-ups, don't solve in standup
- [ ] End on time
- [ ] Blockers assigned owners immediately after

## Framework: Weekly Production Review Structure

### Agenda Template

| Section | Duration | Content |
|---------|----------|---------|
| **Progress** | 15 min | Tasks completed vs. planned, burndown |
| **Risks** | 10 min | Active blockers, emerging risks |
| **Quality** | 10 min | Bug count, stability, test status |
| **Live Ops** (if applicable) | 10 min | Live metrics, event performance |
| **Next Week** | 10 min | Priorities, key deliverables |
| **Decisions** | 5 min | Any decisions needed from group |

### Production Dashboard

| Metric | Target | Current | Trend | Status |
|--------|--------|---------|-------|--------|
| **Progress** | | | | |
| Tasks completed this week | | | ↑↓→ | 🟢🟡🔴 |
| Sprint completion % | | | | |
| **Quality** | | | | |
| Open critical bugs | | | | |
| Test pass rate | | | | |
| Build stability | | | | |
| **Live** (if applicable) | | | | |
| DAU | | | | |
| Revenue | | | | |
| Event participation | | | | |

### Review Roles

| Role | Responsibility |
|------|----------------|
| **Facilitator** (Producer) | Drive agenda, keep time |
| **Note-taker** | Document decisions, action items |
| **Leads** | Report on their area |
| **Stakeholders** | Listen, ask questions |

## Framework: Sprint/Milestone Review

### Demo Session

| Element | Details |
|---------|---------|
| **Duration** | 30-60 min |
| **Attendees** | Full team + stakeholders |
| **Format** | Show completed work, not slides |
| **Focus** | What shipped, not what's coming |
| **Feedback** | Capture for backlog, don't solve live |

### Goal Review

| Goal | Target | Actual | Status | Notes |
|------|--------|--------|--------|-------|
| | | | 🟢🟡🔴 | |
| | | | | |
| | | | | |

### Retrospective

| Question | Findings | Actions |
|----------|----------|---------|
| What went well? | | |
| What didn't go well? | | |
| What should we try? | | |
| What should we stop? | | |

### Action Item Tracking

| Action | Owner | Due | Status |
|--------|-------|-----|--------|
| | | | |
| | | | |

## Framework: Review Health Indicators

| Indicator | Healthy | Warning | Concerning |
|-----------|---------|---------|------------|
| Stand-up duration | <15 min | 15-20 min | >20 min |
| Stand-up attendance | >90% | 75-90% | <75% |
| Blockers resolved | Same day | Within 2 days | >2 days |
| Action items completed | >80% | 50-80% | <50% |
| Review skipped | Never | Rare (vacation) | Regularly |

## Framework: Live Ops Review Addition

For live games, add to weekly review:

| Metric | This Week | Last Week | Target | Action |
|--------|-----------|-----------|--------|--------|
| DAU | | | | |
| D1/D7 Retention | | | | |
| ARPDAU | | | | |
| Event participation | | | | |
| Store rating | | | | |
| Support tickets | | | | |

### Event Performance Review

| Event | Participation | Revenue | Issues | Learnings |
|-------|--------------|---------|--------|-----------|
| | | | | |

## Checklist

- [ ] Daily stand-up format chosen
- [ ] Weekly review agenda defined
- [ ] Production dashboard created
- [ ] Sprint review cadence set
- [ ] Retrospective format chosen
- [ ] Roles assigned
- [ ] Meeting invites sent (recurring)

## Tasks

1. **Choose stand-up format** based on team
2. **Create production dashboard** with key metrics
3. **Schedule recurring meetings** (daily, weekly, sprint)
4. **Define review roles** and expectations
5. **Run first cycle** and iterate on format

## Notes

```
_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________

_______________________________________________________________________________
```

---

# Track A Summary

## Daily Production Checklist

Before proceeding to Block 5 (Scope & Change Management), confirm:

| Production Element | Complete? | Location |
|--------------------|-----------|----------|
| Definition of Done — Features | | |
| Definition of Done — Live Content | | |
| Multi-Level Done Framework | | |
| Task Breakdown Standards | | |
| Work-in-Progress Limits | | |
| Blocker Identification & Escalation | | |
| Build Stability Standards | | |
| Config vs. Code Separation | | |
| Remote Config Management | | |
| QA for Live Content | | |
| Bug Triage Framework | | |
| Hotfix Pipeline | | |
| A/B Test Implementation Standards | | |
| Data Logging Standards | | |
| Daily & Weekly Production Reviews | | |

## Red Flags to Address

- [ ] "Done" means different things to different people
- [ ] Tasks regularly take longer than 2 days
- [ ] Team members juggling 3+ items simultaneously
- [ ] Blockers not surfaced for days
- [ ] Build breaks frequently (>5% failure rate)
- [ ] Can't change anything without client update
- [ ] No staging environment for live content
- [ ] All bugs treated equally regardless of impact
- [ ] No A/B testing capability
- [ ] Missing critical analytics events
- [ ] Reviews skipped or ineffective
