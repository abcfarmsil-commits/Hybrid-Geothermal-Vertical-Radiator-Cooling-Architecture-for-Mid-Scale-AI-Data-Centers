# ABCFarmsIL Repository Organization Guide

This guide outlines the recommended structure for organizing ABCFarmsIL's GitHub repositories and documentation.

---

## 🏗️ Repository Structure Strategy

### Monorepo vs Multi-Repo

**Recommended Approach:** Hybrid Multi-Repo

```
abcfarmsil/
├── abcfarmsil-core/              # Main project repository
├── abcfarmsil-algae-pbr/         # Algae PBR system
├── abcfarmsil-perch-hatchery/    # Yellow Perch hatchery
├── abcfarmsil-microgreens/       # Microgreens production
├── abcfarmsil-controls/          # Control systems and software
└── abcfarmsil-docs/              # Public documentation site
```

**Rationale:**
- **Core repository** for architecture, principles, and shared documentation
- **System-specific repos** for detailed technical specifications and development
- **Controls repo** for software development (separate audience)
- **Docs repo** for public-facing documentation and website

---

## 📁 Core Repository Structure (abcfarmsil-core)

```
abcfarmsil-core/
├── README.md                              # Main project README
├── CONTRIBUTING.md                        # Contribution guidelines
├── LICENSE                                # License information
│
├── architecture/                          # System architecture
│   ├── buried-infrastructure.md          # Underground core design
│   ├── three-zone-water-framework.md     # Water architecture
│   ├── module-integration.md             # System integration
│   └── scalability-strategy.md           # Scaling methodology
│
├── business/                              # Business development
│   ├── VC-supplemental-memo.md           # Investor materials
│   ├── resort-pilot.md                   # Pilot opportunities
│   ├── partnership-proposal.md            # Partnership framework
│   └── market-analysis/                   # Market research
│
├── specifications/                        # Technical specifications
│   ├── BOM_by_Module.md                  # Master Bill of Materials
│   ├── irrigation-specifications.md       # Water delivery specs
│   ├── utility-connections.md            # Utility interface standards
│   └── supplier-illinois.md               # Illinois supply chain
│
├── diagrams/                              # Visual documentation
│   ├── architecture/
│   │   ├── three-zone-flow.svg
│   │   ├── buried-core-layout.svg
│   │   └── module-integration.svg
│   ├── systems/
│   │   ├── algae-pbr-layout.svg
│   │   ├── hatchery-flow.svg
│   │   └── microgreens-zoning.svg
│   └── utilities/
│       ├── plumbing-schematics/
│       ├── electrical-layouts/
│       └── control-network.svg
│
├── deployment/                            # Implementation guides
│   ├── construction-guide.md             # Construction procedures
│   ├── commissioning-checklist.md        # Startup procedures
│   ├── operator-manual.md                 # Daily operations
│   └── maintenance-schedule.md            # Preventive maintenance
│
├── research/                              # Research and references
│   ├── biological-processes/              # Growing systems research
│   ├── water-quality/                     # Aquaculture research
│   ├── energy-efficiency/                 # Energy optimization
│   └── academic-references.md             # Citations and sources
│
├── templates/                             # Reusable templates
│   ├── SOP-template.md                    # Standard Operating Procedures
│   ├── inspection-checklist.md            # Quality control
│   ├── test-plan-template.md              # Testing protocols
│   └── data-recording-form.md             # Data collection
│
└── assets/                                # Static assets
    ├── images/
    ├── models/
    └── specifications/
```

---

## 📁 System-Specific Repository Structure

### Example: abcfarmsil-algae-pbr/

```
abcfarmsil-algae-pbr/
├── README.md                              # System overview
├── CHANGELOG.md                           # Version history
├── LICENSE
│
├── specs/                                 # Technical specifications
│   ├── system-overview.md                 # Complete system description
│   ├── pbr-configuration.md               # PBR panel details
│   ├── lane-isolation.md                  # Flavor lane design
│   └── harvest-process.md                 # Harvesting procedures
│
├── diagrams/                              # System diagrams
│   ├── layout/
│   │   ├── container-layout.svg
│   │   ├── zone-breakdown.svg
│   │   └── plumbing-schematic.svg
│   ├── electrical/
│   │   ├── power-distribution.svg
│   │   ├── led-array-layout.svg
│   │   └── control-system.svg
│   └── flow/
│       ├── media-flow.svg
│       ├── co2-distribution.svg
│       └── cip-system.svg
│
├── software/                              # Control systems
│   ├── plc-programs/                      # PLC logic
│   ├── hmi-designs/                       # Operator interfaces
│   ├── scripts/                           # Automation scripts
│   └── firmware/                          # Device firmware
│
├── testing/                               # Test procedures
│   ├── commissioning-tests.md             # Startup tests
│   ├── performance-tests.md               # Performance benchmarks
│   ├── quality-tests.md                   # Quality assurance
│   └── validation-results.md              # Test data
│
├── operations/                            # Operational procedures
│   ├── startup-procedure.md               # System startup
│   ├── shutdown-procedure.md              # System shutdown
│   ├── daily-routine.md                   # Daily operations
│   └── emergency-procedures.md            # Emergency handling
│
├── maintenance/                           # Maintenance procedures
│   ├── preventive-maintenance.md          # Scheduled maintenance
│   ├── corrective-maintenance.md          # Troubleshooting
│   ├── parts-list.md                      # Spare parts
│   └── calibration-procedures.md          # Sensor calibration
│
└── data/                                  # Data and documentation
    ├── process-parameters/                # Operating parameters
    ├── quality-metrics/                   # Quality data
    ├── performance-logs/                  # Performance logs
    └── batch-records/                     # Production records
```

---

## 📁 Documentation Repository Structure (abcfarmsil-docs)

```
abcfarmsil-docs/
├── README.md                              # Documentation site overview
├── _config.yml                            # Site configuration (Jekyll/Hugo)
│
├── _posts/                                # Blog posts
│   ├── 2026-01-15-welcome.md
│   ├── 2026-01-20-algae-system.md
│   └── ...
│
├── _pages/                                # Static pages
│   ├── about.md
│   ├── systems.md
│   ├── research.md
│   └── contact.md
│
├── _includes/                             # Reusable components
│   ├── header.html
│   ├── footer.html
│   └── navigation.html
│
├── assets/                                # Site assets
│   ├── css/
│   ├── js/
│   └── images/
│
└── docs/                                  # Comprehensive documentation
    ├── getting-started/
    │   ├── overview.md
    │   ├── quick-start.md
    │   └── system-selection.md
    ├── architecture/
    │   ├── buried-infrastructure.md
    │   ├── water-framework.md
    │   └── module-integration.md
    ├── systems/
    │   ├── algae-pbr/
    │   ├── perch-hatchery/
    │   └── microgreens/
    └── resources/
        ├── references/
        ├── glossary/
        └── faq.md
```

---

## 🎯 File Naming Conventions

### General Rules

- **Use lowercase with hyphens:** `three-zone-water-framework.md`
- **Be descriptive:** `commissioning-checklist.md` (not `checklist.md`)
- **Include version for specs:** `BOM_v2.1.md`
- **Date format for logs:** `YYYY-MM-DD`

### Specific Patterns

| Type | Pattern | Example |
|------|---------|---------|
| Documentation | `topic-description.md` | `pbr-configuration.md` |
| Diagrams | `system-component-type.svg` | `algae-pbr-layout.svg` |
| Test Data | `test-system-date.csv` | `performance-algae-2026-01-15.csv` |
| SOPs | `sop-process-name.md` | `sop-harvest-procedure.md` |
| Meeting Notes | `meeting-date-topic.md` | `meeting-2026-01-15-design-review.md` |

---

## 📝 README Templates

### Main Repository README

Each repository should include:

1. **Project title and brief description**
2. **Purpose and scope**
3. **Key features/capabilities**
4. **Quick start guide**
5. **Directory structure overview**
6. **How to contribute**
7. **License information**
8. **Contact information**

### System-Specific README

Include additional sections:

1. **System specifications**
2. **Architecture overview**
3. **Installation/deployment guide**
4. **Operating procedures**
5. **Maintenance requirements**
6. **Troubleshooting guide**

---

## 🔗 Cross-Repository Linking

### Linking Strategy

Use relative links for cross-repository references:

```markdown
For detailed PBR specifications, see [abcfarmsil-algae-pbr](https://github.com/abcfarmsil/abcfarmsil-algae-pbr)
```

### Shared Assets

Store shared assets in the core repository:

```markdown
![Three-zone diagram](https://github.com/abcfarmsil/abcfarmsil-core/raw/main/diagrams/architecture/three-zone-flow.svg)
```

---

## 📊 Documentation Hierarchy

### Priority Levels

**Level 1 - Essential (Must Have):**
- README.md in every repository
- System architecture documentation
- Key technical specifications
- Installation/deployment guides

**Level 2 - Important (Should Have):**
- Operating procedures
- Maintenance procedures
- Troubleshooting guides
- Testing documentation

**Level 3 - Nice to Have (Could Have):**
- Research and references
- Case studies
- White papers
- Educational materials

---

## 🔄 Documentation Maintenance

### Review Schedule

- **README files:** Review quarterly
- **Technical specs:** Review after major changes
- **Procedures:** Review semi-annually
- **Diagrams:** Update with system changes

### Update Process

1. Create branch: `doc-update-description`
2. Make changes following guidelines
3. Update CHANGELOG.md
4. Submit pull request
5. Include review checklist

---

## 🎨 Visual Documentation

### Diagram Standards

- **File format:** SVG (preferred) or high-resolution PNG
- **Naming:** System-component-type.svg
- **Versioning:** Include version in filename for major revisions
- **Accessibility:** Include alt text descriptions

### Diagram Types

**Architecture:**
- System overview diagrams
- Flow charts
- Integration diagrams

**Technical:**
- Plumbing schematics
- Electrical layouts
- Control network diagrams
- Equipment placement drawings

**Process:**
- Flow process diagrams
- Operating procedures
- Maintenance workflows

---

## 📞 Contact

For questions about repository organization or documentation standards, contact the ABCFarmsIL team.

---

## 📄 License

© 2026 ABCFarmsIL. All rights reserved.