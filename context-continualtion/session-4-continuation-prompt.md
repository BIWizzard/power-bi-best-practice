# Power BI Best Practices Guide - Session 4 Continuation Prompt

**Use this prompt to start Session 4 in a new Claude Code conversation**

---

## Session 4 Initialization Prompt

```
I'm continuing development of the Power BI Best Practices Guide for AbsoluteCare healthcare analytics.

CONTEXT DOCUMENTS:
1. Main context: context-continualtion/ideation-setup-context.md
2. Session progress: context-continualtion/session-progress-2025-10-21.md

SESSION 1 ACCOMPLISHMENTS (12 topics complete):
✅ Tier 1 - Priority Quick Wins (5/5 complete)
✅ Tier 2 - Foundation Building (5/5 complete)
- Introduction & Guide Overview, Topic Template

SESSION 2 ACCOMPLISHMENTS (7 topics complete):
✅ Tier 3 - Future State Preparation (5/5 complete)
✅ Tier 4 - Comprehensive Coverage (2 of 20 started)
- 01.3 Relationship Configuration & Cardinality
- 01.4 Calculated Columns vs Measures

SESSION 3 ACCOMPLISHMENTS (5 topics complete):
✅ Performance Optimization & Query Design (category complete):
- 02.2 Data Model Size Reduction
- 02.5 Visual & Page Load Optimization

✅ DAX Development Best Practices (category complete):
- 03.2 Variables & Code Readability
- 03.3 Filter Context & Context Transition
- 03.4 Time Intelligence Patterns

CURRENT STATUS:
- Topics Completed: 24 of 37 (65%)
- Remaining: 13 topics (ALL Tier 4 - Comprehensive Coverage)
- 3 complete categories (Data Architecture, Performance, DAX)
- All completed topics follow standardized template exactly
- Healthcare context integrated throughout
- Assessment findings incorporated in Common Pitfalls sections
- Consistent quality: 5-7 pages per topic with 2+ examples, 3+ pitfalls

IMMEDIATE TASK - FINAL 13 TOPICS:
Complete the guide by writing the following topics to reach 37/37 (100%):

**Report Design & User Experience (3 remaining):**
1. 04.2 - Navigation & Cross-Report Drillthrough
2. 04.3 - Mobile-Responsive Design
3. 04.5 - Accessibility & Color Contrast

**Development Workflow & Version Control (2 remaining):**
4. 05.4 - Testing & Change Management
5. 05.5 - Documentation Standards

**Governance, Security & Deployment (3 remaining):**
6. 06.2 - Workspace Roles & Permissions
7. 06.4 - Data Classification & Sensitivity Labels
8. 06.5 - Usage Monitoring & Adoption

**Continuous Learning & Community Resources (5 remaining):**
9. 07.1 - Essential Books & Publications
10. 07.2 - Top Blogs & Websites
11. 07.3 - LinkedIn Influencers & Thought Leaders
12. 07.4 - Community Forums & User Groups
13. 07.5 - Certification Paths & Training

CRITICAL PROCESS (established in Sessions 1, 2 & 3):
1. Write each topic following _templates/topic-template.md EXACTLY
2. Maintain same quality/detail level as previous sessions (5-7 pages each)
3. After EACH topic completion:
   - Update context-continualtion/session-progress-2025-10-21.md
   - Ask me to check /context
   - I will decide: continue or start new session
4. Use TodoWrite to track progress

QUALITY REQUIREMENTS (from Sessions 1, 2 & 3):
- Follow template structure exactly (Overview, Key Principles, Practical Examples, Common Pitfalls, Healthcare Context, Learn More)
- Include 2+ practical examples with code snippets where applicable
- Include 3+ common pitfalls from assessment or industry best practices
- Integrate healthcare context (performance <5s SLA, print, mobile, HIPAA)
- Cross-link related topics using relative markdown paths
- Cite quality sources (SQLBI, Microsoft, MVPs, community leaders)
- Use healthcare scenarios (patients, encounters, providers, facilities, daily huddles)
- Reference AbsoluteCare assessment findings where relevant

ASSESSMENT TOPICS INTEGRATION:
Already covered: Import migration, One Big Table→star schema, measure rigor, Dev/Test/Prod, version control, deployment pipelines, incremental refresh, relationships, calculated columns, variables, filter context, time intelligence
Still to cover: Field Parameters & Bookmarks (in 04.2), UI/UX patterns (in 04.3, 04.5), documentation standards (in 05.5), sensitivity labels (in 06.4)

FILE PATHS:
- Template: _templates/topic-template.md
- Session progress: context-continualtion/session-progress-2025-10-21.md
- Main context: context-continualtion/ideation-setup-context.md
- Topic files: [Category Folder]/[Topic Number] - [Topic Name].md

Please confirm you've read both context documents and are ready to begin completing the final 13 topics, starting with 04.2 - Navigation & Cross-Report Drillthrough.
```

---

## Quick Reference for Session 4

### Final 13 Topics (Tier 4 - Complete the Guide)

**Report Design & User Experience (3 topics)**

**1. 04.2 - Navigation & Cross-Report Drillthrough**
- Category: Report Design & User Experience
- Focus: Multi-page navigation, drillthrough configuration, cross-report linking
- Healthcare angle: Daily huddle → patient detail workflow, paginated report integration
- Key content: Drillthrough pages, bookmark navigation, buttons with actions, report-to-report navigation, field parameters for dynamic views
- Assessment integration: AbsoluteCare issue with paginated to Power BI drillthrough failing

**2. 04.3 - Mobile-Responsive Design**
- Category: Report Design & User Experience
- Focus: Designing for mobile phone/tablet layouts
- Healthcare angle: Field providers, home health nurses, mobile care coordinators, on-call scenarios
- Key content: Mobile layout creation, touch-optimized visuals, mobile-specific considerations, responsive design patterns, offline considerations
- Assessment integration: Mobile access requirement for field staff

**3. 04.5 - Accessibility & Color Contrast**
- Category: Report Design & User Experience
- Focus: WCAG compliance, accessibility features, inclusive design
- Healthcare angle: Diverse clinical workforce, compliance requirements, color blindness considerations
- Key content: WCAG 2.1 AA standards, color contrast ratios, alt text for visuals, keyboard navigation, screen reader compatibility

**Development Workflow & Version Control (2 topics)**

**4. 05.4 - Testing & Change Management**
- Category: Development Workflow & Version Control
- Focus: Testing strategies, UAT process, change communication
- Healthcare angle: Preventing clinical workflow disruption, validation procedures, go-live protocols
- Key content: UAT process, test data strategies, regression testing, change communication templates, rollback procedures
- Assessment integration: Need for formal testing process before production deployment

**5. 05.5 - Documentation Standards**
- Category: Development Workflow & Version Control
- Focus: Measure descriptions, data dictionaries, report documentation
- Healthcare angle: HIPAA audit trail, knowledge transfer, onboarding new analysts
- Key content: Measure description templates, data lineage documentation, user guides, inline comments, metadata management
- Assessment integration: AbsoluteCare measures lacked descriptions

**Governance, Security & Deployment (3 topics)**

**6. 06.2 - Workspace Roles & Permissions**
- Category: Governance, Security & Deployment
- Focus: Power BI workspace security model, role-based access
- Healthcare angle: PHI access controls, minimum necessary principle (HIPAA)
- Key content: Admin/Member/Contributor/Viewer roles, app permissions, sharing best practices, external user access

**7. 06.4 - Data Classification & Sensitivity Labels**
- Category: Governance, Security & Deployment
- Focus: Microsoft Purview sensitivity labels, data classification
- Healthcare angle: PHI data classification, HIPAA compliance, downstream protection
- Key content: Sensitivity label configuration, automatic vs. manual labeling, label inheritance, compliance policies, auditing

**8. 06.5 - Usage Monitoring & Adoption**
- Category: Governance, Security & Deployment
- Focus: Tracking report usage, measuring user adoption
- Healthcare angle: Clinical engagement metrics, training effectiveness, ROI measurement
- Key content: Power BI activity logs, usage metrics app, adoption strategies, user feedback loops, engagement KPIs

**Continuous Learning & Community Resources (5 topics)**

**9. 07.1 - Essential Books & Publications**
- Category: Continuous Learning & Community Resources
- Focus: Curated book list for Power BI mastery
- Healthcare angle: Healthcare-specific BI books where available
- Key content: "Definitive Guide to DAX" (Russo/Ferrari), "Analyzing Data with Power BI" (Russo/Ferrari), "Storytelling with Data" (Knaflic), "Power BI Performance Best Practices" (Merchant), healthcare analytics books

**10. 07.2 - Top Blogs & Websites**
- Category: Continuous Learning & Community Resources
- Focus: Best online learning resources, staying current
- Healthcare angle: Healthcare BI blogs and case studies
- Key content: SQLBI, Radacad, PowerBI.Tips, Guy in a Cube, Paul Turley's SQL Server BI Blog, Chris Webb's BI Blog, Havens Consulting, Microsoft Power BI Blog

**11. 07.3 - LinkedIn Influencers & Thought Leaders**
- Category: Continuous Learning & Community Resources
- Focus: Who to follow for Power BI expertise and industry trends
- Healthcare angle: Healthcare BI thought leaders where available
- Key content: Marco Russo, Alberto Ferrari, Reza Rad, Patrick LeBlanc, Adam Saxton, Ruth Pozuelo Martinez, Alex Powers, healthcare analytics influencers

**12. 07.4 - Community Forums & User Groups**
- Category: Continuous Learning & Community Resources
- Focus: Where to get help, ask questions, and network
- Healthcare angle: Healthcare BI communities and user groups
- Key content: Power BI Community Forums, Reddit r/PowerBI, LinkedIn groups, local user groups, healthcare analytics communities, virtual meetups

**13. 07.5 - Certification Paths & Training**
- Category: Continuous Learning & Community Resources
- Focus: Professional certifications and structured learning paths
- Healthcare angle: Career development for healthcare BI analysts
- Key content: PL-300 (Power BI Data Analyst), DP-600 (Fabric Analytics Engineer), SQLBI courses, Enterprise DNA, DataCamp, Microsoft Learn paths, study strategies

### Established Patterns (from Sessions 1, 2 & 3)

**Code Examples:**
- DAX: Healthcare scenarios (patients, encounters, providers, readmissions, quality metrics)
- Power Query: Reference ABCDW database (Bronze/Silver/Gold layers)
- SQL: StarSchema views (ABCDW.silver schema)
- Always include before/after comparisons showing improvement
- Performance metrics where applicable

**Healthcare Integration:**
- Performance: Reference <5 second SLA throughout
- Print: Consider daily huddle requirements (8.5x11" layouts)
- Mobile: Field provider scenarios (care coordinators, mobile workflows)
- Compliance: HIPAA/PHI considerations, audit trails
- Real scenarios: Patient census, readmissions, quality metrics, provider attribution

**Cross-Linking:**
- Format: `[Topic Title](../Category%20Folder/Topic%20File.md)`
- Always include 2-4 related topics in Learn More section
- Reference completed topics liberally to build cohesive guide
- URL-encode spaces in folder names: `%20`

**Source Citations:**
- Primary: SQLBI (Marco Russo, Alberto Ferrari)
- Official: Microsoft documentation and Learn portal
- Community: Guy in a Cube, PowerBI.Tips, DAX Patterns
- Books: "Definitive Guide to DAX", "Analyzing Data with Power BI", "Storytelling with Data"
- Healthcare: Healthcare-specific resources where available

**Common Pitfalls:**
- Always include 3-4 pitfalls per topic
- Reference AbsoluteCare assessment findings where relevant
- Include "Impact" statement explaining why pitfall is problematic
- Provide concrete prevention/solution strategies
- Use ❌ or "L" symbol for pitfalls, ✓ for correct approaches

**Topic Length & Quality:**
- 5-7 pages per topic (established in Session 3)
- 2-3 detailed practical examples with code/scenarios
- 3+ common pitfalls with impact statements
- Healthcare Context section with performance/print/mobile/compliance subsections
- Learn More section with 6-10 quality resources organized by type

---

## Session Management Protocol

1. **Start Session**: Read both context documents (main + session progress)
2. **Begin Topics**: Write final 13 topics in order (start with 04.2)
3. **After Each Topic**:
   - Update session-progress-2025-10-21.md with topic summary
   - Ask user to check `/context`
   - User decides: continue or new session
4. **Quality Check**: Every topic matches Sessions 1, 2 & 3 quality/detail
5. **Context Monitoring**: Stop at 75-80% context usage for clean handoff if needed
6. **Goal**: Complete all 13 remaining topics to reach 37/37 (100% COMPLETE!)

---

## Files Modified Per Topic

Per topic completion:
1. New topic file: `[Category]/[Number] - [Name].md`
2. Updated: `context-continualtion/session-progress-2025-10-21.md`

DO NOT modify:
- Main context document (ideation-setup-context.md)
- Template file (already created)
- Session 2 or 3 continuation prompts (historical records)
- README files (update at very end only, after all 37 topics complete)

---

## Success Criteria for Session 4

**Minimum Success**: Complete 6+ topics (bringing total to 30+, 81%)
**Target Success**: Complete 10+ topics (bringing total to 34+, 92%)
**Ideal Success**: Complete all 13 topics (37 of 37, 100% - GUIDE COMPLETE!)

**If all 37 topics completed in Session 4**:
- Mark session-progress-2025-10-21.md as COMPLETE
- Update main README.md with completion status
- Create final summary section in session progress
- Note: Ready for PDF generation using Pandoc (as documented in BUILD-README.md)
- Note: Guide ready for client review and delivery

---

## Special Notes for Category 07 Topics

**Continuous Learning & Community Resources** topics (07.1-07.5) have different format:

**No code examples needed** - These are curated resource lists
**Focus on quality over quantity** - 10-15 highly curated resources per topic
**Organize by subcategory** - Books by topic, blogs by author, etc.
**Include descriptions** - Explain why each resource is valuable
**Healthcare angle** - Highlight healthcare-specific resources where available
**Practical guidance** - How to use these resources (study plans, certification paths)

**Template still applies** but adapted:
- Overview: Why this category of resources matters
- Key Principles: How to evaluate/choose resources in this category
- Practical Examples: Become "Featured Resources" or "Top Recommendations"
- Common Pitfalls: Mistakes in learning approach (e.g., "Jumping to advanced before mastering basics")
- Healthcare Context: Healthcare-specific resources and career considerations
- Learn More: Meta-resources (resource directories, aggregators)

---

**Ready to copy the "Session 4 Initialization Prompt" above and start a new Claude Code session to complete the guide!**
