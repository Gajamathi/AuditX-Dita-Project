# AuditX DITA Documentation Package
## Complete File Inventory and Implementation Guide

**Version:** 1.0  
**Product:** AuditX  
**Creation Date:** September 2026  
**Format:** DITA XML (Darwin Information Typing Architecture)

---

## TABLE OF CONTENTS

1. [Package Overview](#package-overview)
2. [File Inventory](#file-inventory)
3. [DITA Maps](#dita-maps)
4. [Audience-Specific Deliverables](#audience-specific-deliverables)
5. [Publishing Instructions](#publishing-instructions)
6. [Single-Sourcing Architecture](#single-sourcing-architecture)
7. [Customization Guide](#customization-guide)
8. [Support and Maintenance](#support-and-maintenance)

---

## PACKAGE OVERVIEW

### What You Have

This package contains a complete DITA XML documentation system for AuditX product. It implements true single-sourcing, allowing one set of source topics to be published in multiple formats and customized for different audiences.

### Key Features

- **Single-Source Content:** 12 reusable DITA topics
- **Multiple Audiences:** Separate guides for Admin, Supervisor, and Operator roles
- **Multi-Channel Output:** Publish to PDF, HTML, EPUB, Help systems
- **Reusable Components:** Topics assembled into different maps for different purposes
- **Professional Quality:** Follows DITA best practices and standards
- **Fully Editable:** Ready to customize in Oxygen XML Editor or similar tool

### Why DITA?

DITA (Darwin Information Typing Architecture) is an XML-based standard for creating modular, reusable documentation. Benefits for AuditX:

- **Consistency:** Same topic used in multiple places stays in sync
- **Efficiency:** Update once, deploy everywhere
- **Scalability:** Easy to add new topics or workflows as AuditX evolves
- **Professionalism:** Industry-standard format recognized by documentation tools
- **Flexibility:** Output to any format without changing source

---

## FILE INVENTORY

### DITA Topic Files (Concept, Task, Reference)

| File Name | Type | Purpose | Audience |
|-----------|------|---------|----------|
| `auditx-product-overview.dita` | Concept | Introduces AuditX, capabilities, and architecture | Admin, Supervisor, Custom User |
| `auditx-user-roles.dita` | Reference | Defines roles and permission matrices | Admin, Custom User |
| `auditx-reset-password.dita` | Task | Password reset procedure | All Users |
| `auditx-create-site.dita` | Task | How to create an operational site | Admin, Custom User |
| `auditx-create-users.dita` | Task | How to create user accounts | Admin |
| `auditx-workflows-overview.dita` | Concept | Explains workflow types and selection | Admin, Supervisor, Custom User |
| `auditx-create-order-verification-workflow.dita` | Task | Detailed workflow configuration | Admin, Custom User |
| `auditx-reports-reference.dita` | Reference | Report fields, filters, and data | Admin, Supervisor, Custom User |
| `auditx-glossary.dita` | Reference | Term definitions and acronyms | All Users |
| `auditx-troubleshooting.dita` | Reference | Problem-solution troubleshooting | All Users |

**Total Topics:** 10 core topics (ready for expansion)

### DITA Map Files

| File Name | Purpose | Output Type |
|-----------|---------|-------------|
| `auditx-master.ditamap` | Master map - all content in canonical order | Reference/Complete documentation |
| `auditx-admin-guide.ditamap` | Administrator guide | Admin PDF, Admin HTML, Admin Help |
| `auditx-supervisor-guide.ditamap` | Supervisor quick start | Supervisor PDF, Supervisor HTML |
| `auditx-operator-guide.ditamap` | Operator reference card | Operator PDF, Quick Start, Mobile |

### Supporting Documentation

| File Name | Purpose |
|-----------|---------|
| `DITA-ARCHITECTURE-GUIDE.dita` | Complete guide to the DITA structure and publishing |
| `AUDITX-DITA-PACKAGE-README.md` | This file - inventory and usage guide |

**Total Files:** 14 files (10 topics + 4 maps + supporting docs)

---

## DITA MAPS

### Master Map (auditx-master.ditamap)

**Purpose:** Single source of truth containing all AuditX content

**Structure:**
```
Front Matter (TOC, Figures, Tables)
├── Foundational Concepts
│   ├── Product Overview
│   ├── User Roles
│   └── Workflows Overview
├── Getting Started
│   ├── Reset Password
│   ├── Create Site
│   └── Create Users
├── Workflow Configuration
│   └── Order Verification Workflow
├── Reporting
│   └── Reports Reference
└── Back Matter (Glossary, Troubleshooting)
```

**Use:** Generate complete documentation reference

---

### Administrator Guide (auditx-admin-guide.ditamap)

**Purpose:** Comprehensive reference for system administrators

**Audience Filter:** `administrator`, `custom-user`

**Sections:**
1. Getting Started as Administrator
2. System Initialization and Setup
3. Configuring Workflows
4. Advanced Configuration
5. Monitoring, Reporting, and Maintenance

**Typical Size:** 50-80 pages (PDF)

**Outputs:** PDF manual, HTML portal, Embedded help

---

### Supervisor Guide (auditx-supervisor-guide.ditamap)

**Purpose:** Operations supervisor quick reference

**Audience Filter:** `supervisor`

**Sections:**
1. Welcome to AuditX
2. Understanding the Supervisor Role
3. Understanding Workflows
4. Monitoring Operations and Accessing Reports

**Typical Size:** 15-20 pages (PDF)

**Outputs:** Quick Start PDF, Mobile HTML, Dashboard guide

---

### Operator Guide (auditx-operator-guide.ditamap)

**Purpose:** Packing floor operator quick reference

**Audience Filter:** `operator`

**Sections:**
1. Welcome Operator
2. Understanding Your Role
3. Using the AuditX Device

**Typical Size:** 4-6 pages (laminated card or PDF)

**Outputs:** Quick reference card, Mobile app, Touchscreen guide

---

## AUDIENCE-SPECIFIC DELIVERABLES

### For Administrators

**Content Included:**
- Complete system overview
- All configuration procedures
- Advanced features (webhooks, config groups, ROI)
- Troubleshooting with admin-level solutions
- Complete glossary

**Recommended Outputs:**
- PDF: 60-80 page Administrator's Manual (printed and digital)
- HTML: Web-based help portal with search
- CHM: Windows Help file for offline access
- EPUB: E-book format for tablets/readers

**Distribution Channels:**
- Email to IT/Admin team
- Internal wiki or documentation portal
- Printed manual at server room
- Help system integrated in Forge application

---

### For Supervisors

**Content Included:**
- Product overview (read-only)
- Workflow overview (understanding what happens)
- Complete reports section
- Basic troubleshooting

**Excludes:**
- All configuration procedures
- Admin-only tasks
- Operator procedures
- Advanced technical details

**Recommended Outputs:**
- PDF: 15-20 page Quick Start guide
- HTML: Mobile-friendly web reference
- Laminated reference card: Key report features and filters

**Distribution Channels:**
- Email to supervisor team
- Printed poster near supervisor workstations
- Mobile app for on-floor access
- Dashboard integration tips

---

### For Operators

**Content Included:**
- Product purpose (why they're using it)
- Role and responsibilities
- Workflow overview (from operator perspective)
- Quick troubleshooting for device issues

**Excludes:**
- All configuration
- Admin procedures
- Report analysis (supervisor task)
- Advanced settings

**Recommended Outputs:**
- Laminated quick reference card (4x6 inches): Most common steps
- Mobile PDF: Quick start on tablet at packing station
- Touchscreen guide: Integrated help in device UI
- Video tutorial: Step-by-step device operation

**Distribution Channels:**
- Laminated cards at each packing station
- Mobile app on tablets provided to operators
- Printed quick start with first-day training
- Help system in device touchscreen interface

---

## PUBLISHING INSTRUCTIONS

### Prerequisites

You'll need one of these tools to publish DITA:

1. **Oxygen XML Editor** (Recommended - Full GUI)
   - Commercial tool with excellent DITA support
   - Includes DITA transformation engine
   - Can publish to PDF, HTML, WebHelp, EPUB
   - Available at: https://www.oxygenxml.com

2. **DITA Open Toolkit (DITA OT)** (Free)
   - Open-source tool
   - Command-line interface
   - Supports PDF, HTML, HTML5, WebHelp, EPUB
   - Download: https://www.dita-ot.org

3. **Other Tools**
   - Adobe FrameMaker (advanced features)
   - XMetaL (enterprise)
   - AuthorIT (specialized)

### Publishing with Oxygen XML Editor

#### Step 1: Open the Map File
```
File → Open → [Select auditx-admin-guide.ditamap]
```

#### Step 2: Select Transformation Scenario
```
Right-click on map → Apply Transformation Scenario
OR
Window → Show View → Transformation Scenarios
```

#### Step 3: Choose Output Format
- **PDF**: Select "DITA Map PDF" scenario
- **HTML**: Select "DITA Map HTML5" scenario
- **WebHelp**: Select "DITA Map WebHelp Responsive" scenario

#### Step 4: Configure Output Settings
- Output folder: `/output/auditx-admin-guide`
- Customize XSLT parameters if needed (branding, colors, etc.)

#### Step 5: Run Transformation
```
Click "Apply" or "Apply and Close"
Wait for transformation to complete
Check output folder for generated files
```

### Publishing with DITA Open Toolkit (Command Line)

#### Installation
```bash
# Download and extract DITA OT
cd ~/dita-ot-4.0
```

#### Generate Administrator PDF
```bash
dita -i /auditx-dita/auditx-admin-guide.ditamap \
     -f pdf \
     -o /output/auditx-admin-guide
```

#### Generate Supervisor HTML
```bash
dita -i /auditx-dita/auditx-supervisor-guide.ditamap \
     -f html5 \
     -o /output/auditx-supervisor-guide
```

#### Generate Operator Quick Reference
```bash
dita -i /auditx-dita/auditx-operator-guide.ditamap \
     -f pdf \
     -o /output/auditx-operator-quick-ref \
     -Dargs.pdf.d4p.responsive.enabled=true
```

### Output Quality Assurance

After publishing, verify:

1. **Completeness**
   - All expected topics included
   - No broken links
   - All cross-references valid
   - TOC matches actual content

2. **Audience Filtering**
   - Check that audience-specific content appears/disappears correctly
   - Operator guide should not contain admin tasks
   - Supervisor guide should only include read-only features

3. **Formatting**
   - PDF: Page breaks, margins, headers/footers
   - HTML: Links functional, images load, responsive design
   - Readability: Font sizes, line spacing, color contrast

4. **Search Functionality**
   - PDF: PDF viewer can search
   - HTML: Search box functional
   - Help: Integrated search working

---

## SINGLE-SOURCING ARCHITECTURE

### Content Reuse Strategy

**Principle:** Write once, use multiple times

#### Example 1: Product Overview
```
Single Source: auditx-product-overview.dita
↓
Used in Maps:
  ├── auditx-master.ditamap
  ├── auditx-admin-guide.ditamap
  ├── auditx-supervisor-guide.ditamap
  └── auditx-operator-guide.ditamap
↓
Final Deliverables:
  ├── Administrator Manual (PDF, HTML, Help)
  ├── Supervisor Quick Start (PDF, HTML)
  └── Operator Guide (PDF, Mobile)
```

**Benefit:** Update the overview once, all guides automatically reflect changes

#### Example 2: Password Reset Task
```
Single Source: auditx-reset-password.dita
↓
Included in:
  ├── Master map
  ├── Admin guide (Part 1: Getting Started)
  ├── Supervisor guide (Part 1: Welcome)
  └── Operator guide (Part 1: Welcome)
↓
One source serves all audiences
```

### Profiling Attributes

The architecture uses DITA profiling attributes to control content visibility:

```xml
<topicref href="auditx-create-users.dita">
  <topicmeta>
    <audience type="administrator"/>
  </topicmeta>
</topicref>
```

**Audience Values:**
- `administrator` - System admin and IT staff
- `custom-user` - Custom/sub-admin users  
- `supervisor` - Operations supervisors
- `operator` - Packing floor operators
- `all-users` - Everyone

When publishing, specify which audiences to include:
```bash
dita -i auditx-admin-guide.ditamap \
     -f pdf \
     -Dargs.filter=admin-filter.ditaval
```

---

## CUSTOMIZATION GUIDE

### Adding New Workflows

When AuditX adds new features (e.g., Image Logging workflow):

#### Step 1: Create New Task Topic
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE task PUBLIC "-//OASIS//DTD DITA Task//EN" "task.dtd">
<task id="auditx_create_image_logging_workflow">
  <title>Create an Image Logging Workflow</title>
  ...
</task>
```

Save as: `auditx-create-image-logging-workflow.dita`

#### Step 2: Add to Master Map
```xml
<topicref href="auditx-create-image-logging-workflow.dita" type="task">
  <topicmeta>
    <audience type="administrator"/>
    <audience type="custom-user"/>
    <data name="workflow-type" value="image-logging"/>
  </topicmeta>
</topicref>
```

#### Step 3: Add to Relevant Maps
Add the same topicref to:
- `auditx-admin-guide.ditamap` (in Workflow Configuration section)

#### Step 4: Regenerate Outputs
```bash
dita -i auditx-admin-guide.ditamap -f pdf -o /output
dita -i auditx-master.ditamap -f html5 -o /output
```

### Updating Existing Topics

When fixing errors or updating information:

#### Step 1: Edit the Source Topic
```xml
<!-- Edit auditx-create-site.dita -->
<step>
  <cmd>Enter the site name with location details</cmd>
  <info>... updated information ...</info>
</step>
```

#### Step 2: Review Related Topics
Check other topics that reference this one for consistency

#### Step 3: Regenerate All Maps
```bash
# Regenerate all outputs
./rebuild-all-guides.sh
```

#### Step 4: QA Test
- Verify changes appear in all relevant deliverables
- Test PDF, HTML, and Help outputs
- Check cross-references still work

### Creating New Maps

To create a guide for a new audience (e.g., Implementation Partners):

#### Step 1: Create New Map File
```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE map PUBLIC "-//OASIS//DTD DITA Map//EN" "map.dtd">
<map id="auditx_partner_guide">
  <title>AuditX Implementation Partner Guide</title>
  <topicmeta>
    <audience type="implementation-partner"/>
  </topicmeta>
  
  <topicref href="auditx-product-overview.dita"/>
  <!-- ... add relevant topics ... -->
</map>
```

Save as: `auditx-partner-guide.ditamap`

#### Step 2: Reference Relevant Topics
Include existing topics with appropriate profiling

#### Step 3: Add Profiling to Topics
```xml
<topicref href="auditx-create-config-groups.dita">
  <topicmeta>
    <audience type="implementation-partner"/>
  </topicmeta>
</topicref>
```

#### Step 4: Generate New Outputs
```bash
dita -i auditx-partner-guide.ditamap -f pdf -o /output
```

---

## SUPPORT AND MAINTENANCE

### Version Management

Track changes using version control (Git, SVN):

```bash
# Commit new workflow
git add auditx-create-video-recording-workflow.dita
git add auditx-admin-guide.ditamap
git commit -m "Add Video Recording workflow documentation"
git tag -a v1.1 -m "Release 1.1: Added Video Recording workflow"
```

### Regular Maintenance Schedule

**Monthly:**
- Review support tickets for documentation gaps
- Update troubleshooting section with new issues

**Quarterly:**
- Review all screenshots/figures for accuracy
- Update version numbers and dates
- Check for broken links

**Annually:**
- Comprehensive review of all content
- Rewrite outdated procedures
- Add new features and capabilities
- Regenerate all outputs

### Expanding the Documentation

**Coming Soon (Placeholders):**
- Video Recording Workflow task
- Image Logging Workflow task
- Webhook Configuration task
- Config Group Creation task
- ROI Configuration task
- System Assignment task
- User-to-Site Assignment task
- Activity Logs reference
- API Logs reference

Each can be created following the same structure and added to relevant maps.

### Oxygen XML Customization

To customize the look and feel in Oxygen:

1. Create custom CSS or XSL files
2. Reference in transformation scenario
3. Apply branding (colors, fonts, logos)
4. Generate branded outputs

### Support Contacts

For DITA-related questions:
- **Oxygen Support:** https://www.oxygenxml.com/support.html
- **DITA OT Community:** https://dita-ot.org/contribute
- **DITA TC:** https://www.oasis-open.org/committees/dita/

---

## QUICK START CHECKLIST

- [ ] Extract all DITA files to working directory
- [ ] Install Oxygen XML Editor or DITA OT
- [ ] Open `auditx-master.ditamap` to review structure
- [ ] Generate PDF for Administrator guide
- [ ] Test HTML output for Supervisor guide
- [ ] Review generated documents for completeness
- [ ] Customize branding/styling as needed
- [ ] Deploy outputs to distribution channels
- [ ] Train content authors on DITA process
- [ ] Set up version control repository
- [ ] Plan schedule for ongoing maintenance

---

## CONCLUSION

This DITA documentation system provides a professional, scalable foundation for AuditX documentation. By following single-sourcing principles, you can maintain high-quality documentation efficiently while supporting multiple audiences and delivery channels.

**For additional support or customization:**
- Consult the DITA-ARCHITECTURE-GUIDE.dita for detailed technical information
- Contact Oxygen vendor for tool-specific training
- Reference DITA.ot.org for open-source toolkit documentation

---

**Document Version:** 1.0  
**Last Updated:** September 2026  
**Status:** Ready for Production Use
