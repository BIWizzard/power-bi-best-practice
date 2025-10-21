# Power BI Best Practices Guide - Session 2 Continuation Prompt

**Use this prompt to start Session 2 in a new Claude Code conversation**

---

## Session 2 Initialization Prompt

```
I'm continuing development of the Power BI Best Practices Guide for AbsoluteCare healthcare analytics.

CONTEXT DOCUMENTS:
1. Main context: context-continualtion/ideation-setup-context.md
2. Session 1 progress: context-continualtion/session-progress-2025-10-21.md

SESSION 1 ACCOMPLISHMENTS (12 topics complete):
✅ Tier 1 - Priority Quick Wins (5/5 complete)
- 02.4 Performance Analyzer Workflow
- 04.4 Print-Friendly Layouts for Healthcare
- 02.1 Query Folding & Import vs DirectQuery
- 03.5 Common DAX Anti-patterns
- 01.2 Fact vs Dimension Tables

✅ Tier 2 - Foundation Building (5/5 complete)
- 01.1 Star Schema Design Principles
- 03.1 Measure Organization & Naming Conventions
- 05.1 Dev/Test/Prod Workspace Strategy
- 06.1 Row-Level Security Patterns
- 04.1 Visual Selection Guide

Plus: Introduction & Guide Overview, Topic Template

CURRENT STATUS:
- Topics Completed: 12 of 37 (32%)
- Remaining: 25 topics (5 Tier 3 + 20 Tier 4)
- All completed topics follow standardized template exactly
- Healthcare context integrated throughout
- Assessment findings incorporated in Common Pitfalls sections

IMMEDIATE TASK - TIER 3 (Future State Preparation):
Write the following 5 topics IN THIS ORDER:
1. 01.5 - Bridging to Medallion Architecture
2. 05.3 - Version Control for Power BI
3. 06.3 - Deployment Pipelines & CI-CD
4. 02.3 - Incremental Refresh Strategies
5. 05.2 - External Tools - Tabular Editor & DAX Studio

CRITICAL PROCESS (established in Session 1):
1. Write each topic following _templates/topic-template.md EXACTLY
2. Maintain same quality/detail level as Session 1 topics (3-4 pages each)
3. After EACH topic completion:
   - Update context-continualtion/session-progress-2025-10-21.md
   - Ask me to check /context
   - I will decide: continue or start new session
4. Use TodoWrite to track progress

QUALITY REQUIREMENTS (from Session 1):
- Follow template structure exactly (Overview, Key Principles, Practical Examples, Common Pitfalls, Healthcare Context, Learn More)
- Include 2+ practical examples with code snippets
- Include 3+ common pitfalls from assessment
- Integrate healthcare context (performance <5s SLA, print, mobile, HIPAA)
- Cross-link related topics using relative markdown paths
- Cite quality sources (SQLBI, Microsoft, MVPs)
- Use healthcare scenarios (patients, encounters, providers, facilities, daily huddles)
- Reference AbsoluteCare assessment findings where relevant

ASSESSMENT TOPICS INTEGRATION:
Already covered: Import migration, One Big Table→star schema, measure rigor, Dev/Test/Prod
Still to cover: Date table/Time Intelligence (in 03.4), Field Parameters & Bookmarks (in UX topics), UI/UX patterns (in design topics)

FILE PATHS:
- Template: _templates/topic-template.md
- Session progress: context-continualtion/session-progress-2025-10-21.md
- Main context: context-continualtion/ideation-setup-context.md
- Topic files: [Category Folder]/[Topic Number] - [Topic Name].md

Please confirm you've read both context documents and are ready to begin with 01.5 - Bridging to Medallion Architecture.
```

---

## Quick Reference for Session 2

### Next 5 Topics (Tier 3)

**1. 01.5 - Bridging to Medallion Architecture**
- Category: Data Architecture & Semantic Modeling
- Focus: Preparing for Bronze/Silver/Gold data layers
- Healthcare angle: Future-proofing current star schema for migration
- Key content: Medallion architecture overview, current state assessment, incremental adoption path

**2. 05.3 - Version Control for Power BI**
- Category: Development Workflow & Version Control
- Focus: Git integration for .pbix files, using external tools
- Healthcare angle: Change tracking for compliance, team collaboration
- Key content: Tabular Editor Git workflow, .pbix vs .bim files, branching strategies

**3. 06.3 - Deployment Pipelines & CI-CD**
- Category: Governance, Security & Deployment
- Focus: Automated deployment, Premium pipelines feature
- Healthcare angle: Reducing deployment errors, audit trail
- Key content: Deployment pipeline setup, automation with Azure DevOps, deployment rules

**4. 02.3 - Incremental Refresh Strategies**
- Category: Performance Optimization & Query Design
- Focus: Large-scale data refresh optimization
- Healthcare angle: Multi-year patient data, efficient refresh windows
- Key content: Incremental refresh configuration, RangeStart/RangeEnd parameters, partition strategies

**5. 05.2 - External Tools - Tabular Editor & DAX Studio**
- Category: Development Workflow & Version Control
- Focus: Advanced development and optimization tools
- Healthcare angle: Performance tuning, bulk operations on measures
- Key content: Tabular Editor features, DAX Studio query analysis, Best Practice Analyzer

### After Tier 3 (Next Steps)

**Tier 4 - Comprehensive Coverage (20 topics)**
Remaining topics across all categories to complete the 37-topic guide.

### Established Patterns

**Code Examples:**
- DAX: Healthcare scenarios (patients, encounters, providers)
- Power Query: Reference ABCDW database
- SQL: StarSchema views
- Always include before/after comparisons

**Healthcare Integration:**
- Performance: Reference <5 second SLA throughout
- Print: Consider daily huddle requirements
- Mobile: Field provider scenarios
- Compliance: HIPAA/PHI considerations

**Cross-Linking:**
- Format: `[Topic Title](../Category%20Folder/Topic%20File.md)`
- Always include 2-4 related topics in Learn More section

**Source Citations:**
- Primary: SQLBI (Marco Russo, Alberto Ferrari)
- Official: Microsoft documentation
- Community: Guy in a Cube, PowerBI.Tips, DAX Patterns
- Books: "Definitive Guide to DAX", "Analyzing Data with Power BI"

---

## Session Management Protocol

1. **Start Session**: Read both context documents (main + session progress)
2. **Begin Topics**: Write Tier 3 topics in order
3. **After Each Topic**:
   - Update session-progress-2025-10-21.md with topic summary
   - Ask user to check `/context`
   - User decides: continue or new session
4. **Quality Check**: Every topic matches Session 1 quality/detail
5. **Context Monitoring**: Stop at 80-85% context usage for clean handoff

---

## Files Modified Per Topic

Per topic completion:
1. New topic file: `[Category]/[Number] - [Name].md`
2. Updated: `context-continualtion/session-progress-2025-10-21.md`

DO NOT modify:
- Main context document (ideation-setup-context.md)
- Template file (already created)
- README files (update at end only)

---

**Ready to copy the "Session 2 Initialization Prompt" above and start a new Claude Code session.**
