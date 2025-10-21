# Power BI Best Practices Guide - Session 3 Continuation Prompt

**Use this prompt to start Session 3 in a new Claude Code conversation**

---

## Session 3 Initialization Prompt

```
I'm continuing development of the Power BI Best Practices Guide for AbsoluteCare healthcare analytics.

CONTEXT DOCUMENTS:
1. Main context: context-continualtion/ideation-setup-context.md
2. Session progress: context-continualtion/session-progress-2025-10-21.md

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

SESSION 2 ACCOMPLISHMENTS (7 topics complete):
✅ Tier 3 - Future State Preparation (5/5 complete)
- 01.5 Bridging to Medallion Architecture
- 05.3 Version Control for Power BI
- 06.3 Deployment Pipelines & CI-CD
- 02.3 Incremental Refresh Strategies
- 05.2 External Tools - Tabular Editor & DAX Studio

✅ Tier 4 - Comprehensive Coverage (2 of 20 started)
- 01.3 Relationship Configuration & Cardinality
- 01.4 Calculated Columns vs Measures

CURRENT STATUS:
- Topics Completed: 19 of 37 (51%)
- Remaining: 18 topics (ALL Tier 4 - Comprehensive Coverage)
- All completed topics follow standardized template exactly
- Healthcare context integrated throughout
- Assessment findings incorporated in Common Pitfalls sections
- Consistent quality: 3-5 pages per topic with 2+ examples, 3+ pitfalls

IMMEDIATE TASK - TIER 4 (Comprehensive Coverage):
Write the following 18 topics to complete the guide:

**Data Architecture & Semantic Modeling (0 remaining - category complete)**

**Performance Optimization & Query Design (2 remaining):**
1. 02.2 - Data Model Size Reduction
2. 02.5 - Visual & Page Load Optimization

**DAX Development Best Practices (3 remaining):**
3. 03.2 - Variables & Code Readability
4. 03.3 - Filter Context & Context Transition
5. 03.4 - Time Intelligence Patterns

**Report Design & User Experience (3 remaining):**
6. 04.2 - Navigation & Cross-Report Drillthrough
7. 04.3 - Mobile-Responsive Design
8. 04.5 - Accessibility & Color Contrast

**Development Workflow & Version Control (2 remaining):**
9. 05.4 - Testing & Change Management
10. 05.5 - Documentation Standards

**Governance, Security & Deployment (3 remaining):**
11. 06.2 - Workspace Roles & Permissions
12. 06.4 - Data Classification & Sensitivity Labels
13. 06.5 - Usage Monitoring & Adoption

**Continuous Learning & Community Resources (5 remaining):**
14. 07.1 - Essential Books & Publications
15. 07.2 - Top Blogs & Websites
16. 07.3 - LinkedIn Influencers & Thought Leaders
17. 07.4 - Community Forums & User Groups
18. 07.5 - Certification Paths & Training

CRITICAL PROCESS (established in Sessions 1 & 2):
1. Write each topic following _templates/topic-template.md EXACTLY
2. Maintain same quality/detail level as previous sessions (3-5 pages each)
3. After EACH topic completion:
   - Update context-continualtion/session-progress-2025-10-21.md
   - Ask me to check /context
   - I will decide: continue or start new session
4. Use TodoWrite to track progress

QUALITY REQUIREMENTS (from Sessions 1 & 2):
- Follow template structure exactly (Overview, Key Principles, Practical Examples, Common Pitfalls, Healthcare Context, Learn More)
- Include 2+ practical examples with code snippets
- Include 3+ common pitfalls from assessment
- Integrate healthcare context (performance <5s SLA, print, mobile, HIPAA)
- Cross-link related topics using relative markdown paths
- Cite quality sources (SQLBI, Microsoft, MVPs)
- Use healthcare scenarios (patients, encounters, providers, facilities, daily huddles)
- Reference AbsoluteCare assessment findings where relevant

ASSESSMENT TOPICS INTEGRATION:
Already covered: Import migration, One Big Table→star schema, measure rigor, Dev/Test/Prod, version control, deployment pipelines, incremental refresh, relationships, calculated columns
Still to cover: Date table/Time Intelligence (in 03.4), Field Parameters & Bookmarks (in 04.2), UI/UX patterns (in 04.3, 04.5), documentation standards (in 05.5)

FILE PATHS:
- Template: _templates/topic-template.md
- Session progress: context-continualtion/session-progress-2025-10-21.md
- Main context: context-continualtion/ideation-setup-context.md
- Topic files: [Category Folder]/[Topic Number] - [Topic Name].md

Please confirm you've read both context documents and are ready to begin completing the remaining 18 Tier 4 topics, starting with 02.2 - Data Model Size Reduction.
```

---

## Quick Reference for Session 3

### Remaining Topics (Tier 4 - 18 topics)

**Performance Optimization (2 topics)**

**1. 02.2 - Data Model Size Reduction**
- Category: Performance Optimization & Query Design
- Focus: Minimizing model size for faster loading and refresh
- Healthcare angle: Large patient/encounter datasets, year-over-year growth
- Key content: Column pruning, datatype optimization, avoiding calculated columns, aggregation tables

**2. 02.5 - Visual & Page Load Optimization**
- Category: Performance Optimization & Query Design
- Focus: Optimizing visual performance beyond DAX optimization
- Healthcare angle: Meeting <5 second SLA for clinical dashboards
- Key content: Visual limits, page load strategies, bookmarks vs. hidden visuals, lazy loading

**DAX Development (3 topics)**

**3. 03.2 - Variables & Code Readability**
- Category: DAX Development Best Practices
- Focus: Using VAR to improve DAX maintainability and performance
- Healthcare angle: Complex clinical calculations, team collaboration
- Key content: Variable benefits, performance gains (eliminating redundant calculations), debugging, measure documentation

**4. 03.3 - Filter Context & Context Transition**
- Category: DAX Development Best Practices
- Focus: Understanding how filter context works in DAX evaluation
- Healthcare angle: Patient attribution, provider filtering, time period analysis
- Key content: Row context vs filter context, CALCULATE context transition, ALLSELECTED vs ALL

**5. 03.4 - Time Intelligence Patterns**
- Category: DAX Development Best Practices
- Focus: Date tables and time-based calculations
- Healthcare angle: YTD metrics, prior year comparisons, rolling averages
- Key content: Date table requirements, TOTALYTD, SAMEPERIODLASTYEAR, custom fiscal calendars

**Report Design & UX (3 topics)**

**6. 04.2 - Navigation & Cross-Report Drillthrough**
- Category: Report Design & User Experience
- Focus: Multi-page navigation and cross-report linking
- Healthcare angle: Daily huddle → patient detail workflow, paginated report integration
- Key content: Drillthrough configuration, bookmarks, buttons, report-to-report navigation

**7. 04.3 - Mobile-Responsive Design**
- Category: Report Design & User Experience
- Focus: Designing for mobile phone layouts
- Healthcare angle: Field providers, mobile care management, on-call scenarios
- Key content: Mobile layout creation, touch-optimized visuals, mobile-specific considerations

**8. 04.5 - Accessibility & Color Contrast**
- Category: Report Design & User Experience
- Focus: WCAG compliance, accessibility features
- Healthcare angle: Diverse clinical workforce, compliance requirements
- Key content: Color blindness considerations, alt text, keyboard navigation, WCAG 2.1 standards

**Development Workflow (2 topics)**

**9. 05.4 - Testing & Change Management**
- Category: Development Workflow & Version Control
- Focus: Testing strategies before production deployment
- Healthcare angle: Preventing clinical workflow disruption, validation procedures
- Key content: UAT process, test data strategies, regression testing, change communication

**10. 05.5 - Documentation Standards**
- Category: Development Workflow & Version Control
- Focus: Measure descriptions, data dictionaries, report documentation
- Healthcare angle: HIPAA audit trail, knowledge transfer, onboarding
- Key content: Measure description templates, data lineage documentation, user guides

**Governance & Security (3 topics)**

**11. 06.2 - Workspace Roles & Permissions**
- Category: Governance, Security & Deployment
- Focus: Power BI workspace security model
- Healthcare angle: PHI access controls, minimum necessary principle
- Key content: Admin/Member/Contributor/Viewer roles, app permissions, sharing best practices

**12. 06.4 - Data Classification & Sensitivity Labels**
- Category: Governance, Security & Deployment
- Focus: Microsoft Purview sensitivity labels
- Healthcare angle: PHI data classification, HIPAA compliance
- Key content: Sensitivity label configuration, downstream protection, compliance policies

**13. 06.5 - Usage Monitoring & Adoption**
- Category: Governance, Security & Deployment
- Focus: Tracking report usage and user adoption
- Healthcare angle: Clinical engagement metrics, training effectiveness
- Key content: Power BI activity logs, usage metrics app, adoption strategies

**Learning Resources (5 topics)**

**14. 07.1 - Essential Books & Publications**
- Category: Continuous Learning & Community Resources
- Focus: Curated book list for Power BI mastery
- Healthcare angle: Healthcare-specific BI books where available
- Key content: "Definitive Guide to DAX", "Analyzing Data with Power BI", "Storytelling with Data"

**15. 07.2 - Top Blogs & Websites**
- Category: Continuous Learning & Community Resources
- Focus: Best online learning resources
- Healthcare angle: Healthcare BI blogs and case studies
- Key content: SQLBI, Radacad, PowerBI.Tips, Guy in a Cube, Paul Turley

**16. 07.3 - LinkedIn Influencers & Thought Leaders**
- Category: Continuous Learning & Community Resources
- Focus: Who to follow for Power BI expertise
- Healthcare angle: Healthcare BI thought leaders
- Key content: Marco Russo, Alberto Ferrari, Reza Rad, Patrick LeBlanc, Ruth Pozuelo Martinez

**17. 07.4 - Community Forums & User Groups**
- Category: Continuous Learning & Community Resources
- Focus: Where to get help and network
- Healthcare angle: Healthcare BI communities
- Key content: Power BI Community Forums, Reddit r/PowerBI, LinkedIn groups, local user groups

**18. 07.5 - Certification Paths & Training**
- Category: Continuous Learning & Community Resources
- Focus: Professional certifications and structured learning
- Healthcare angle: Career development for healthcare BI analysts
- Key content: PL-300, DP-600, SQLBI courses, Enterprise DNA, DataCamp

### Established Patterns (from Sessions 1 & 2)

**Code Examples:**
- DAX: Healthcare scenarios (patients, encounters, providers, readmissions, quality metrics)
- Power Query: Reference ABCDW database (Bronze/Silver/Gold layers)
- SQL: StarSchema views (ABCDW.silver schema)
- Always include before/after comparisons showing improvement

**Healthcare Integration:**
- Performance: Reference <5 second SLA throughout
- Print: Consider daily huddle requirements (8.5x11" layouts)
- Mobile: Field provider scenarios (care coordinators, mobile workflows)
- Compliance: HIPAA/PHI considerations, audit trails

**Cross-Linking:**
- Format: `[Topic Title](../Category%20Folder/Topic%20File.md)`
- Always include 2-4 related topics in Learn More section
- Reference completed topics liberally to build cohesive guide

**Source Citations:**
- Primary: SQLBI (Marco Russo, Alberto Ferrari)
- Official: Microsoft documentation and Learn portal
- Community: Guy in a Cube, PowerBI.Tips, DAX Patterns
- Books: "Definitive Guide to DAX", "Analyzing Data with Power BI", "Storytelling with Data"

**Common Pitfalls:**
- Always include 3-4 pitfalls per topic
- Reference AbsoluteCare assessment findings where relevant
- Include "Impact" statement explaining why pitfall is problematic
- Provide concrete prevention/solution strategies

---

## Session Management Protocol

1. **Start Session**: Read both context documents (main + session progress)
2. **Begin Topics**: Write Tier 4 topics in order (start with 02.2)
3. **After Each Topic**:
   - Update session-progress-2025-10-21.md with topic summary
   - Ask user to check `/context`
   - User decides: continue or new session
4. **Quality Check**: Every topic matches Sessions 1 & 2 quality/detail
5. **Context Monitoring**: Stop at 75-80% context usage for clean handoff if needed
6. **Goal**: Complete all 18 remaining topics if context allows, or set up clean handoff for Session 4

---

## Files Modified Per Topic

Per topic completion:
1. New topic file: `[Category]/[Number] - [Name].md`
2. Updated: `context-continualtion/session-progress-2025-10-21.md`

DO NOT modify:
- Main context document (ideation-setup-context.md)
- Template file (already created)
- Session 2 continuation prompt (historical record)
- README files (update at very end only, after all 37 topics complete)

---

## Success Criteria for Session 3

**Minimum Success**: Complete 8+ topics (bringing total to 27+, 73%)
**Target Success**: Complete 12+ topics (bringing total to 31+, 84%)
**Ideal Success**: Complete all 18 topics (37 of 37, 100% - GUIDE COMPLETE!)

**If all 37 topics completed**:
- Update main README.md with completion status
- Consider creating final summary document
- Ready for PDF generation using Pandoc

---

**Ready to copy the "Session 3 Initialization Prompt" above and start a new Claude Code session.**
