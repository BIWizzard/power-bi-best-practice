# Power BI Best Practices Guide - Context Continuation Document

**Project**: AbsoluteCare Power BI Best Practices Guide Development  
**Transition Point**: Moving from ideation/planning to content development in Claude Code  
**Date**: October 21, 2025  
**GitHub Repository**: https://github.com/BIWizzard/power-bi-best-practice  
**Primary Branch**: main  
**Status**: Repository structure created, ready for content development

---

## Executive Summary

This document provides complete context for continuing the Power BI Best Practices Guide project in Claude Code. The guide is a comprehensive reference for AbsoluteCare's Power BI development team (approximately 5 developers with ~1 year Power BI experience each) following a consulting engagement where 4 medium-complexity Power BI reports were assessed.

### Project Objectives
1. **Create healthcare-specific best practices guide** for Power BI development
2. **Provide practical, actionable guidance** (not academic theory)
3. **Bridge current state to future state** (team preparing for medallion architecture migration)
4. **Establish ongoing learning resources** (books, blogs, influencers, certifications)
5. **Deliver as interactive PDF** with hyperlinks and optional markdown for internal wiki

### Current State
- ✅ Repository created with complete folder structure (7 categories, 35 topics)
- ✅ Supporting files created (README, .gitignore, BUILD-README)
- ✅ Content structure finalized and validated
- ⏳ **NEXT**: Begin writing topic content using standardized template

---

## Repository Structure

### GitHub Repository Details
- **Repo URL**: https://github.com/BIWizzard/power-bi-best-practice
- **Owner**: BIWizzard
- **Branch**: main
- **Purpose**: Version-controlled markdown source files for best practices guide
- **Output**: Will generate PDF using Pandoc or MkDocs

### File Organization

```
power-bi-best-practice/
├── 00 - Introduction & Guide Overview.md          [EMPTY - needs content]
├── README.md                                       [COMPLETE]
├── .gitignore                                      [COMPLETE]
├── BUILD-README.md                                 [COMPLETE]
│
├── 01 - Data Architecture & Semantic Modeling/
│   ├── 01.1 - Star Schema Design Principles.md           [EMPTY]
│   ├── 01.2 - Fact vs Dimension Tables.md                [EMPTY]
│   ├── 01.3 - Relationship Configuration & Cardinality.md [EMPTY]
│   ├── 01.4 - Calculated Columns vs Measures.md          [EMPTY]
│   └── 01.5 - Bridging to Medallion Architecture.md      [EMPTY]
│
├── 02 - Performance Optimization & Query Design/
│   ├── 02.1 - Query Folding & Import vs DirectQuery.md   [EMPTY]
│   ├── 02.2 - Data Model Size Reduction.md               [EMPTY]
│   ├── 02.3 - Incremental Refresh Strategies.md          [EMPTY]
│   ├── 02.4 - Performance Analyzer Workflow.md           [EMPTY]
│   └── 02.5 - Visual & Page Load Optimization.md         [EMPTY]
│
├── 03 - DAX Development Best Practices/
│   ├── 03.1 - Measure Organization & Naming Conventions.md [EMPTY]
│   ├── 03.2 - Variables & Code Readability.md              [EMPTY]
│   ├── 03.3 - Filter Context & Context Transition.md       [EMPTY]
│   ├── 03.4 - Time Intelligence Patterns.md                [EMPTY]
│   └── 03.5 - Common DAX Anti-patterns.md                  [EMPTY]
│
├── 04 - Report Design & User Experience/
│   ├── 04.1 - Visual Selection Guide.md                    [EMPTY]
│   ├── 04.2 - Navigation & Cross-Report Drillthrough.md    [EMPTY]
│   ├── 04.3 - Mobile-Responsive Design.md                  [EMPTY]
│   ├── 04.4 - Print-Friendly Layouts for Healthcare.md     [EMPTY]
│   └── 04.5 - Accessibility & Color Contrast.md            [EMPTY]
│
├── 05 - Development Workflow & Version Control/
│   ├── 05.1 - Dev Test Prod Workspace Strategy.md          [EMPTY]
│   ├── 05.2 - External Tools - Tabular Editor & DAX Studio.md [EMPTY]
│   ├── 05.3 - Version Control for Power BI.md              [EMPTY]
│   ├── 05.4 - Testing & Change Management.md               [EMPTY]
│   └── 05.5 - Documentation Standards.md                   [EMPTY]
│
├── 06 - Governance Security & Deployment/
│   ├── 06.1 - Row-Level Security Patterns.md               [EMPTY]
│   ├── 06.2 - Workspace Roles & Permissions.md             [EMPTY]
│   ├── 06.3 - Deployment Pipelines & CI-CD.md              [EMPTY]
│   ├── 06.4 - Data Classification & Sensitivity Labels.md  [EMPTY]
│   └── 06.5 - Usage Monitoring & Adoption.md               [EMPTY]
│
├── 07 - Continuous Learning & Community Resources/
│   ├── 07.1 - Essential Books & Publications.md            [EMPTY]
│   ├── 07.2 - Top Blogs & Websites.md                      [EMPTY]
│   ├── 07.3 - LinkedIn Influencers & Thought Leaders.md    [EMPTY]
│   ├── 07.4 - Community Forums & User Groups.md            [EMPTY]
│   └── 07.5 - Certification Paths & Training.md            [EMPTY]
│
├── _assets/
│   ├── images/          [EMPTY - for screenshots, diagrams]
│   ├── diagrams/        [EMPTY - for architectural diagrams]
│   └── code-examples/   [EMPTY - for DAX snippets, M code examples]
│
└── _templates/
    └── topic-template.md [NEEDS CREATION - standardized content structure]
```

---

## Content Strategy & Standards

### Guide Scope & Sizing
- **Target Length**: 70-105 pages (2-3 pages per topic)
- **Level 1 Categories**: 7 (optimal for comprehensive coverage without overwhelm)
- **Level 2 Topics**: 35 total (5 per category - focused and scannable)
- **Level 3**: Selective deep-dives only where complexity warrants (e.g., Time Intelligence, RLS, Visual Selection)

### Audience Profile
- **Experience Level**: ~1 year Power BI development experience
- **Team Size**: 5 developers
- **Organization**: AbsoluteCare (healthcare analytics, mobile care management)
- **Context**: Recently assessed 4 medium-complexity Power BI reports
- **Future State**: Preparing for medallion architecture migration
- **Learning Style**: Eager learners, quick adopters, ask good questions

### Healthcare-Specific Considerations
**CRITICAL**: Every topic must consider healthcare operational context:

1. **Performance Requirements**
   - Target: <5 second load times (clinical workflow SLA)
   - Context: Providers abandoning slow reports, workflow disruption
   - Impact: Patient care delays

2. **Print Requirements**
   - Use Case: Pixel-perfect printed reports for daily huddles
   - Current: Using paginated reports for critical huddle materials
   - Goal: Power BI alternatives maintaining print quality

3. **Mobile Usage**
   - Context: Providers accessing reports in field/patient locations
   - Need: Mobile-responsive designs, offline capability considerations

4. **Compliance**
   - HIPAA considerations in all recommendations
   - PHI handling and security
   - Audit trail requirements

5. **Cross-Report Navigation**
   - Issue: Drill-through from paginated to Power BI reports currently failing
   - Impact: Fragmented user experience
   - Priority: Unified navigation strategy

### Delivery Medium: Hybrid PDF + Markdown

**Primary Deliverable**: Interactive PDF with extensive hyperlinking
- Universally accessible (works offline, SharePoint-friendly)
- Supports active hyperlinks, bookmarks, table of contents
- Professional consulting deliverable format
- No hosting dependency required
- Version controllable

**Bonus Deliverable**: Source markdown files
- Enables future internal wiki creation (SharePoint/Teams)
- Future-proofs content for their adaptation
- Demonstrates knowledge transfer best practices

**Creation Tools**:
- Author in Markdown (portability, version control)
- Use **Pandoc** or **MkDocs** to generate:
  - Beautiful hyperlinked PDF (primary delivery)
  - Optional static HTML files (internal hosting)

---

## Standardized Topic Template

**CRITICAL**: Every Level 2 topic must follow this exact structure for consistency and usability.

### Template Structure (1-2 pages per topic)

```markdown
# [Topic Number] - [Topic Name]

## Overview
[2-3 sentences explaining what this topic covers and why it matters for healthcare analytics]

## Key Principles
[3-5 focused bullet points covering core concepts or rules]

- **Principle 1**: Brief explanation
- **Principle 2**: Brief explanation  
- **Principle 3**: Brief explanation
- **Principle 4**: Brief explanation
- **Principle 5**: Brief explanation (if needed)

## Practical Example

### Example 1: [Descriptive Title]
[Concrete example with code snippets, screenshots, or diagrams where relevant]

```dax
// Example DAX code
Total Sales = SUM(Sales[Amount])
```

**Why this works**: [Brief explanation of the principle in action]

### Example 2: [Descriptive Title] (if needed)
[Additional example showing before/after comparison or alternative approach]

## Common Pitfalls

### ❌ Pitfall 1: [What to Avoid]
[Brief description of common mistake]
**Impact**: [Why this is problematic]

### ❌ Pitfall 2: [What to Avoid]
[Brief description of common mistake]
**Impact**: [Why this is problematic]

### ❌ Pitfall 3: [What to Avoid] (if needed)
[Brief description of common mistake]
**Impact**: [Why this is problematic]

## Healthcare Context

### Performance Considerations
[How this topic impacts the <5 second load time SLA]

### Print/Mobile Implications
[Specific considerations for printed huddle reports or mobile access - if applicable]

### Compliance Notes
[HIPAA or security considerations - if applicable]

## Learn More

### Official Documentation
- [Link to Microsoft documentation] - [Brief description]

### Expert Resources
- [Link to expert blog/article] - [Brief description]

### Video Content
- [Link to tutorial/demo] - [Brief description]

### Related Topics
- [Internal link to related topic within guide]
- [Internal link to related topic within guide]

---

*Last updated: [Date]*
```

### Template Usage Notes

1. **Consistency is King**: Use this template for ALL 35 topics without deviation
2. **Healthcare Integration**: Don't isolate healthcare considerations - weave throughout
3. **Practical Over Academic**: Show, don't just tell
4. **Cite Quality Sources**: 
   - Prioritize: Microsoft official docs, SQLBI, MVP blogs
   - Include: Books (Marco Russo, Alberto Ferrari), community resources
   - Avoid: Generic tutorials, uncredited content

5. **Internal Linking**: Use markdown relative links for cross-references
   - Example: `See [Star Schema Design](../01%20-%20Data%20Architecture/01.1%20-%20Star%20Schema%20Design%20Principles.md)`

6. **Code Examples**: 
   - Always include DAX/M code in proper code blocks
   - Add comments explaining key parts
   - Show both "before" and "after" where relevant

7. **Visual Assets**:
   - Screenshots go in `_assets/images/`
   - Diagrams go in `_assets/diagrams/`
   - Reference using relative paths: `![Description](_assets/images/screenshot.png)`

---

## Assessment Findings to Incorporate

The guide must reflect insights from the 4 Power BI report assessments conducted:

### Performance Issues Identified
1. **DAX Optimization Needs**
   - Inefficient measures causing slow load times
   - Lack of variable usage for code reusability
   - Context transition issues

2. **Data Model Problems**
   - Non-optimal star schema implementation
   - Relationship cardinality issues
   - Calculated columns where measures should be used

3. **Query Folding Gaps**
   - DirectQuery performance issues
   - Query folding breaks in Power Query
   - Unnecessary data transfer

### UX/Design Findings
1. **Print Requirements Not Met**
   - Reports don't translate well to printed format for huddles
   - Relying on paginated reports as workaround

2. **Navigation Fragmentation**
   - Drill-through from paginated to Power BI failing
   - Inconsistent cross-report navigation patterns

3. **Mobile Responsiveness Lacking**
   - Reports not optimized for field provider access

### Governance Gaps
1. **Workspace Organization**
   - Dev/Test/Prod strategy not clearly defined
   - Security and permission management inconsistent

2. **Version Control Absent**
   - No systematic approach to tracking changes
   - Risk of lost work or unclear history

3. **Documentation Sparse**
   - Limited measure documentation
   - Data model relationships not explained

**Action**: Weave these findings into "Common Pitfalls" and "Healthcare Context" sections throughout guide

---

## Priority Topics for Quick Wins

These topics should be prioritized because they address immediate pain points from the assessment:

### Tier 1 - Immediate Impact (Write First)
1. **02.4 - Performance Analyzer Workflow** 
   - Addresses critical performance issues
   - Directly applicable to their current slow reports
   
2. **04.4 - Print-Friendly Layouts for Healthcare**
   - Solves daily operational pain point
   - Unique healthcare requirement

3. **02.1 - Query Folding & Import vs DirectQuery**
   - Major performance improvement opportunity
   - Current DirectQuery issues identified

4. **03.5 - Common DAX Anti-patterns**
   - Can immediately improve existing measures
   - Lots of assessment examples to draw from

5. **01.2 - Fact vs Dimension Tables**
   - Foundational for data model improvements
   - Prepares for medallion architecture

### Tier 2 - Foundation Building (Write Second)
6. **01.1 - Star Schema Design Principles**
7. **03.1 - Measure Organization & Naming Conventions**
8. **05.1 - Dev Test Prod Workspace Strategy**
9. **06.1 - Row-Level Security Patterns**
10. **04.1 - Visual Selection Guide**

### Tier 3 - Future State Preparation (Write Third)
11. **01.5 - Bridging to Medallion Architecture**
12. **05.3 - Version Control for Power BI**
13. **06.3 - Deployment Pipelines & CI-CD**
14. **02.3 - Incremental Refresh Strategies**
15. **05.2 - External Tools - Tabular Editor & DAX Studio**

### Tier 4 - Comprehensive Coverage (Write Last)
16-35. All remaining topics following the category order

---

## Key Source Materials & References

### AbsoluteCare Project Context
**Available in Claude Desktop Project Files**:
- `Provider_PQ` - Power Query dimension table creation
- `Patient_NQ` - Native SQL query for patient dimension
- `Care_Facts` - Fact table with multiple provider lookups
- `Duplicate Patient Chat Transcript` - Discussion on deduplication, surrogate keys, query folding
- `AbsoluteCare_PowerBI_SOW_v1_0_20250702__fully_executed_20250703.pdf` - Statement of Work
- `AbsoluteCare_Trace3_Scope.png` - Visual scope summary
- `Initial email from Project Manager` - Project kickoff context
- `one_list_results_membership.csv` - Sample data structure

**Key Insights from Transcripts**:
- Team discussion on star schema vs denormalized tables
- Query folding challenges in DirectQuery mode
- Native SQL vs Power Query tradeoffs
- Surrogate key stability concerns
- SMI Care Pathway population selection criteria

### Essential External References

#### Books (Must Reference)
1. **"The Definitive Guide to DAX" by Marco Russo & Alberto Ferrari** (SQLBI)
   - Bible for DAX development
   - Reference for: 03.3, 03.4, 03.5

2. **"Analyzing Data with Power BI and Power Pivot for Excel" by Alberto Ferrari & Marco Russo**
   - Data modeling fundamentals
   - Reference for: 01.1, 01.2, 01.3

3. **"Power BI Performance Best Practices" by Bhavik Merchant**
   - Performance optimization deep-dive
   - Reference for: All of Category 02

4. **"Storytelling with Data" by Cole Nussbaumer Knaflic**
   - Visualization principles
   - Reference for: 04.1, 04.5

#### Online Resources (Curate Best)
1. **SQLBI** (https://www.sqlbi.com)
   - Marco Russo, Alberto Ferrari articles
   - DAX patterns library
   - Video courses

2. **Microsoft Power BI Documentation**
   - Official best practices
   - Performance tuning guides
   - Security implementation

3. **Power BI Community Forums**
   - Real-world problem solving
   - Community patterns

4. **DAX.guide** (https://dax.guide)
   - DAX function reference
   - Examples and patterns

#### LinkedIn Influencers to Feature (Category 07.3)
- Marco Russo (SQLBI co-founder, DAX expert)
- Alberto Ferrari (SQLBI co-founder, data modeling)
- Reza Rad (Power BI MVP, trainer)
- Patrick LeBlanc (Microsoft, Guy in a Cube)
- Adam Saxton (Microsoft, Guy in a Cube)
- Melissa Coates (data architecture, sadly passed 2021 - mention legacy)
- Ruth Pozuelo Martinez (Power BI tips, DAX)
- Alex Powers (data viz specialist)

#### Blogs to Feature (Category 07.2)
- SQLBI Blog
- Radacad Blog (Reza Rad)
- PowerBI.Tips
- Guy in a Cube (Microsoft)
- Paul Turley's SQL Server BI Blog
- Chris Webb's BI Blog
- Havens Consulting

#### Certifications to Feature (Category 07.5)
- **PL-300**: Microsoft Power BI Data Analyst
- **DP-600**: Implementing Analytics Solutions Using Microsoft Fabric
- **DA-100** (retired, replaced by PL-300)
- SQLBI courses (DAX, data modeling)
- Enterprise DNA courses

---

## Technical Specifications

### Markdown Standards
- **Headers**: Use ATX-style (`#`, `##`, `###`)
- **Code Blocks**: Always specify language (```dax, ```powerquery, ```sql)
- **Links**: Use reference-style for repeated URLs
- **Images**: Use relative paths from current file location
- **Lists**: Use `-` for unordered, `1.` for ordered
- **Emphasis**: Use `**bold**` for key terms, `*italic*` for emphasis

### Git Workflow
```bash
# Standard commit pattern
git add [file]
git commit -m "feat: [Category] - [Topic Title] - [Brief description]"

# Examples:
git commit -m "feat: Performance - Add Query Folding topic with healthcare examples"
git commit -m "docs: Update README with completion status"
git commit -m "fix: Correct DAX syntax in Time Intelligence examples"
```

### PDF Generation (When Content Complete)

#### Using Pandoc (Recommended)
```bash
pandoc "00 - Introduction & Guide Overview.md" \
  "01 - Data Architecture & Semantic Modeling"/*.md \
  "02 - Performance Optimization & Query Design"/*.md \
  "03 - DAX Development Best Practices"/*.md \
  "04 - Report Design & User Experience"/*.md \
  "05 - Development Workflow & Version Control"/*.md \
  "06 - Governance Security & Deployment"/*.md \
  "07 - Continuous Learning & Community Resources"/*.md \
  --toc \
  --toc-depth=2 \
  --number-sections \
  --pdf-engine=xelatex \
  -V geometry:margin=1in \
  -V linkcolor:blue \
  -V urlcolor:blue \
  -V documentclass=report \
  -V fontsize=11pt \
  --metadata title="Power BI Best Practices Guide for Healthcare Analytics" \
  --metadata subtitle="AbsoluteCare Development Team Reference" \
  --metadata author="Trace3 Consulting - Ken Gallagher" \
  --metadata date="$(date +%B\ %Y)" \
  -o "AbsoluteCare_PowerBI_Best_Practices_Guide.pdf"
```

#### Using MkDocs (Alternative for Web + PDF)
1. Create `mkdocs.yml` configuration
2. Run `mkdocs build` for static site
3. Use `mkdocs-with-pdf` plugin for PDF generation
4. Optional: Deploy to GitHub Pages for online access

---

## Content Development Workflow

### Phase 1: Foundation (Estimated 1-2 days)
1. **Create topic template** (`_templates/topic-template.md`)
2. **Write Introduction** (`00 - Introduction & Guide Overview.md`)
   - Welcome and how to use guide
   - AbsoluteCare context and assessment overview
   - Guide structure explanation
   - Healthcare-specific focus areas

3. **Test template** with one complete topic (suggest: 02.4 - Performance Analyzer)
   - Validate template structure
   - Ensure healthcare context integration
   - Confirm hyperlink approach
   - Generate sample PDF to test output

### Phase 2: Priority Topics (Estimated 2-3 days)
4. **Write Tier 1 topics** (5 topics addressing immediate pain points)
   - Use assessment findings for Common Pitfalls
   - Include screenshots/diagrams where beneficial
   - Cross-link related topics

5. **Review and refine** after Tier 1 complete
   - Ensure consistency across topics
   - Check healthcare integration
   - Validate code examples
   - Test internal linking

### Phase 3: Comprehensive Coverage (Estimated 3-4 days)
6. **Write Tier 2 topics** (Foundation building - 5 topics)
7. **Write Tier 3 topics** (Future state preparation - 5 topics)
8. **Write Tier 4 topics** (Comprehensive coverage - 20 topics)

### Phase 4: Community Resources (Estimated 1 day)
9. **Write Category 07** (Continuous Learning - 5 topics)
   - Curate best books, blogs, influencers
   - Provide specific learning paths
   - Include certification roadmap

### Phase 5: Polish & Delivery (Estimated 1 day)
10. **Final review and editing**
    - Consistency check across all topics
    - Hyperlink validation
    - Code syntax verification
    - Grammar and clarity pass

11. **Generate PDF deliverable**
    - Test Pandoc/MkDocs output
    - Verify table of contents
    - Check hyperlink functionality
    - Ensure images render correctly

12. **Package for delivery**
    - Final PDF for AbsoluteCare team
    - Source markdown files (optional)
    - Build instructions (BUILD-README.md)
    - Git repository access

**Total Estimated Effort**: 8-11 business days (based on 5-7 topics per day)

---

## Success Criteria

### Content Quality Metrics
- [ ] All 35 topics follow standardized template exactly
- [ ] Healthcare context integrated in 100% of applicable topics
- [ ] Each topic includes 1-2 practical examples with code/screenshots
- [ ] Each topic includes 2-3 common pitfalls from assessment
- [ ] Each topic includes 2-3 curated external learning resources
- [ ] Internal cross-linking present throughout guide
- [ ] All DAX/M code examples are syntactically correct
- [ ] All external links are valid and current

### Healthcare-Specific Requirements
- [ ] Performance considerations (<5 sec SLA) addressed in relevant topics
- [ ] Print requirements addressed explicitly in UX section
- [ ] Mobile usage patterns discussed in relevant topics
- [ ] HIPAA/compliance considerations integrated throughout
- [ ] Cross-report navigation issues acknowledged and addressed
- [ ] Medallion architecture bridge clearly explained

### Deliverable Quality
- [ ] PDF generates cleanly without errors
- [ ] Table of contents is comprehensive and hyperlinked
- [ ] All internal links work correctly in PDF
- [ ] All external links are clickable in PDF
- [ ] Images and diagrams render properly
- [ ] Page breaks are logical and readable
- [ ] Professional formatting throughout
- [ ] Code examples are syntax-highlighted

### Business Value
- [ ] Addresses all major findings from 4-report assessment
- [ ] Provides immediate actionable guidance (quick wins)
- [ ] Establishes foundation for long-term improvement
- [ ] Supports upcoming medallion architecture migration
- [ ] Creates ongoing learning pathway for team
- [ ] Serves as living document (maintainable/updatable)

---

## Known Constraints & Considerations

### Time Constraints
- **Scope**: Up to 4 medium complexity reports per SOW
- **Timeline**: 6-8 weeks total engagement (guide is final deliverable)
- **Effort**: Estimated 8-11 business days for guide completion

### Technical Constraints
- **Environment**: AbsoluteCare uses DirectQuery heavily
- **Tools**: Power BI Service, ABCDW database, healthcare clinical reporting
- **User Base**: ~75-100 providers across organization
- **Infrastructure**: Medicon prod/test workspaces, OIE production

### Scope Boundaries (From SOW)
**In Scope**:
- Review best practices and performance benchmarks
- Assessment of data accuracy and user experience
- Document feedback and develop improvement plan
- Report design standards, data modeling, performance, governance

**Out of Scope**:
- Data migration or protection services
- Ongoing support or maintenance
- Working on open support issues
- Implementation of recommendations (guidance only)

---

## Claude Code Session Initialization Prompt

**Use this prompt to begin the Claude Code session after saving this context document:**

```
I'm continuing development of a Power BI Best Practices Guide for a healthcare analytics consulting engagement with AbsoluteCare. 

CONTEXT DOCUMENT: I have a comprehensive context document at context-continuation/ideation-setup-context.md that contains:
- Complete project background and objectives
- Repository structure (GitHub: https://github.com/BIWizzard/power-bi-best-practice)
- Standardized topic template that MUST be followed exactly
- Healthcare-specific requirements (print, performance, mobile, compliance)
- Assessment findings to incorporate
- Priority order for topic development
- Success criteria and quality metrics

CURRENT STATE:
- Repository structure is complete (7 categories, 35 empty topic files)
- Supporting files exist (README, .gitignore, BUILD-README)
- Ready to begin content development

IMMEDIATE TASK:
1. Read the context document thoroughly
2. Create the topic template file at _templates/topic-template.md
3. Write the Introduction file (00 - Introduction & Guide Overview.md)
4. Then begin with Priority Tier 1 topics in this order:
   - 02.4 - Performance Analyzer Workflow
   - 04.4 - Print-Friendly Layouts for Healthcare
   - 02.1 - Query Folding & Import vs DirectQuery
   - 03.5 - Common DAX Anti-patterns
   - 01.2 - Fact vs Dimension Tables

CRITICAL REQUIREMENTS:
- Follow the standardized template EXACTLY for every topic
- Integrate healthcare context throughout (don't isolate it)
- Include practical examples with code snippets
- Cite quality sources (SQLBI, Microsoft, MVP blogs)
- Use assessment findings in "Common Pitfalls" sections
- Maintain professional but practical tone (not academic)
- Cross-link related topics using markdown relative links

DELIVERABLE:
- 70-105 page comprehensive guide (2-3 pages per topic)
- Interactive PDF with hyperlinks
- Markdown source files in Git repository

Please confirm you've read the context document and are ready to begin with the template creation.
```

---

## Post-Completion Checklist

After completing guide development in Claude Code:

### Pre-Delivery Review
- [ ] All 35 topics completed and follow template
- [ ] Introduction provides clear guide overview
- [ ] Healthcare context integrated throughout
- [ ] All code examples tested for syntax
- [ ] All external links validated
- [ ] All internal cross-references working
- [ ] Git repository committed and pushed

### PDF Generation
- [ ] Pandoc successfully generates PDF
- [ ] Table of contents is complete
- [ ] All hyperlinks functional
- [ ] Images render correctly
- [ ] Page breaks are logical
- [ ] Professional appearance confirmed

### Client Handoff Preparation
- [ ] PDF uploaded to SharePoint/delivery location
- [ ] GitHub repository access instructions provided
- [ ] BUILD-README.md reviewed and accurate
- [ ] Optional: Presentation deck summarizing guide highlights
- [ ] Optional: Recorded walkthrough of key topics

### Project Closeout
- [ ] Completion certificate drafted
- [ ] Deliverable signed off by AbsoluteCare stakeholders
- [ ] Lessons learned documented
- [ ] Repository archived or transferred to client

---

## Contact Information & Stakeholders

### Primary Contacts (from SOW)
- **Rob Posner** - Chief Technology Officer (Client Sponsor)
- **Thomas Wilson** - Business lead, primary contact for scope/priority
- **Hannah Mannering** - Technical lead for Member 360 app (SMI Care Pathway)
- **Alex Puccio** - Member 360 business lead, print requirements expert

### Trace3 Team
- **Ken Gallagher** - Senior Power BI Consultant (Guide Author)
- **Joe Milien** - Account Manager
- **Mike Garabelli** - Service Delivery Manager

---

## Appendix: Quick Reference

### Markdown Cheat Sheet for Guide
```markdown
# Level 1 Header (Category)
## Level 2 Header (Section)
### Level 3 Header (Subsection)

**Bold text** for key terms
*Italic text* for emphasis

- Unordered list item
- Another item

1. Ordered list item
2. Another item

[Link text](https://example.com)
[Internal link](../folder/file.md)

![Image alt text](_assets/images/screenshot.png)

```dax
// DAX code block
Measure = CALCULATE(...)
```

```powerquery
// Power Query M code block
Source = ...
```

> Blockquote for important callouts

---
Horizontal rule for section breaks
```

### Git Commands Quick Reference
```bash
# Check status
git status

# Stage changes
git add .
git add specific-file.md

# Commit
git commit -m "feat: Add topic on [subject]"

# Push to GitHub
git push origin main

# View history
git log --oneline

# Create branch for experimentation
git checkout -b feature/experimental-topic
```

### File Path Examples
```markdown
# From topic file to template
../_templates/topic-template.md

# From topic to image
../_assets/images/performance-analyzer-screenshot.png

# Cross-reference to another topic
../01%20-%20Data%20Architecture/01.1%20-%20Star%20Schema%20Design%20Principles.md

# Or using anchor links for same file
[See Key Principles](#key-principles)
```

---

**Document Version**: 1.0  
**Created**: October 21, 2025  
**Author**: Ken Gallagher (BIWizzard), Trace3 Senior Power BI Consultant  
**Purpose**: Context continuation for Claude Code development session  
**Status**: Ready for Claude Code handoff  

---

*This document contains all necessary context to seamlessly continue Power BI Best Practices Guide development. No additional context files should be needed.*