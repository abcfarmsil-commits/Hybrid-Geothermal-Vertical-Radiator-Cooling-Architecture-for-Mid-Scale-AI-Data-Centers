# ABCFarmsIL GitHub - Quick Reference

One-page reference guide for ABCFarmsIL GitHub setup and documentation.

---

## 📦 Created Documents

| Document | Purpose | Use When |
|----------|---------|----------|
| `ABCFARMSIL_GITHUB_README.md` | Main project overview | First time visitors, investors |
| `ALGAE_PBR_SYSTEM_README.md` | Algae PBR technical specs | Engineers, operators |
| `YELLOW_PERCH_HATCHERY_README.md` | Hatchery technical specs | Aquaculture specialists |
| `CONTRIBUTING_GUIDELINES.md` | Contribution rules | External collaborators |
| `REPOSITORY_ORGANIZATION.md` | Repo structure guide | Setting up repositories |
| `GITHUB_SETUP_QUICKSTART.md` | Step-by-step setup | Initial GitHub setup |

---

## 🚀 Quick Setup Steps

### 1. Create Account
- Username: `abcfarmsil`
- Profile: Add logo, bio, website

### 2. Create Organization (Optional)
- Go to: `github.com/organizations/new`
- Name: `abcfarmsil`

### 3. Create Repositories
```bash
# Core Repository
Name: abcfarmsil-core
Desc: Main project repository
README: ABCFARMSIL_GITHUB_README.md

# Algae PBR System
Name: abcfarmsil-algae-pbr
Desc: 53-ft reefer container algae PBR
README: ALGAE_PBR_SYSTEM_README.md

# Yellow Perch Hatchery
Name: abcfarmsil-perch-hatchery
Desc: 53-ft reefer container perch hatchery
README: YELLOW_PERCH_HATCHERY_README.md

# Documentation
Name: abcfarmsil-docs
Desc: Public documentation site
README: See GITHUB_SETUP_QUICKSTART.md
```

### 4. Configure Settings
- **Branch Protection:** Enable for `main` branch
- **Topics:** Add relevant tags (see full guide)
- **License:** Choose appropriate license
- **CODEOWNERS:** Add review assignments

---

## 📁 Repository Structure

```
abcfarmsil-core/
├── README.md
├── CONTRIBUTING.md
├── architecture/          # System design docs
├── business/              # Business development
├── specifications/        # Technical specs
├── diagrams/              # Visual documentation
├── deployment/            # Implementation guides
└── research/              # Research & references
```

---

## 🎯 File Naming Rules

- **Use lowercase with hyphens:** `three-zone-water-framework.md`
- **Be descriptive:** `commissioning-checklist.md`
- **Include version:** `BOM_v2.1.md`
- **Date format:** `YYYY-MM-DD`

---

## 🔗 Cross-Repo Links

```markdown
[Algae PBR](https://github.com/abcfarmsil/abcfarmsil-algae-pbr)
[Hatchery](https://github.com/abcfarmsil/abcfarmsil-perch-hatchery)
[Docs](https://github.com/abcfarmsil/abcfarmsil-docs)
```

---

## 📊 Documentation Priority

**Level 1 - Essential:**
- README.md (all repos)
- System architecture
- Key technical specs
- Installation guides

**Level 2 - Important:**
- Operating procedures
- Maintenance procedures
- Troubleshooting guides
- Testing documentation

**Level 3 - Nice to Have:**
- Research references
- Case studies
- Educational materials

---

## ✅ Initial Commit Checklist

- [ ] README files created
- [ ] CONTRIBUTING.md added
- [ ] License files added
- [ ] Repository topics configured
- [ ] Settings configured
- [ ] Branch protection enabled
- [ ] Initial issues created
- [ ] Cross-repo links verified

---

## 📞 Contact

- **GitHub:** https://github.com/abcfarmsil
- **Email:** [Add contact email]
- **Website:** [Add website]

---

## 📄 License

© 2026 ABCFarmsIL. All rights reserved.

---

**For detailed instructions, see:** `GITHUB_SETUP_QUICKSTART.md`