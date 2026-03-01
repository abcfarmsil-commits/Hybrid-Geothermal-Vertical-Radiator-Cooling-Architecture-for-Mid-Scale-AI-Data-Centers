# ABCFarmsIL GitHub Setup - Quick Start Guide

This guide walks you through setting up ABCFarmsIL's GitHub repositories from scratch.

---

## 🚀 Step 1: Account Setup

### Create GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Choose username: `abcfarmsil` (or similar)
4. Complete account verification
5. Set up two-factor authentication (recommended)

### Configure Profile
1. Go to Settings → Profile
2. Upload organization/logo image
3. Add bio: "Regenerative Agricultural Infrastructure - Modular, gravity-first systems for climate resilience and scalable food production."
4. Add website link (when available)
5. Set email visibility to public or private as preferred

---

## 🏢 Step 2: Create Organization (Optional but Recommended)

### Benefits of Organization Account
- Multiple collaborators
- Centralized billing
- Professional appearance
- Team management
- Repository organization

### Create Organization
1. Go to [github.com/organizations/new](https://github.com/organizations/new)
2. Organization name: `abcfarmsil`
3. Organization email: Use primary email
4. Choose free plan initially
5. Complete organization profile

---

## 📦 Step 3: Create Repositories

### Repository 1: Core Repository

**Name:** `abcfarmsil-core`
**Description:** Main project repository for ABCFarmsIL regenerative agricultural infrastructure
**Visibility:** Public
**Initialize with:**
- ✅ README.md
- ✅ .gitignore (Select Python/General)
- ✅ License (Choose appropriate license)

**Add initial files:**
1. Copy `ABCFARMSIL_GITHUB_README.md` → `README.md`
2. Copy `CONTRIBUTING_GUIDELINES.md` → `CONTRIBUTING.md`
3. Copy `REPOSITORY_ORGANIZATION.md` → `docs/repository-organization.md`

### Repository 2: Algae PBR System

**Name:** `abcfarmsil-algae-pbr`
**Description:** 53-ft reefer container fresh algae photobioreactor system
**Visibility:** Public
**Initialize with:**
- ✅ README.md
- ✅ .gitignore
- ✅ License

**Add initial files:**
1. Copy `ALGAE_PBR_SYSTEM_README.md` → `README.md`

### Repository 3: Yellow Perch Hatchery

**Name:** `abcfarmsil-perch-hatchery`
**Description:** 53-ft reefer container yellow perch breeding, spawning, and nursery system
**Visibility:** Public
**Initialize with:**
- ✅ README.md
- ✅ .gitignore
- ✅ License

**Add initial files:**
1. Copy `YELLOW_PERCH_HATCHERY_README.md` → `README.md`

---

## 📁 Step 4: Create Documentation Repository

**Name:** `abcfarmsil-docs`
**Description:** Public documentation site for ABCFarmsIL systems
**Visibility:** Public
**Initialize with:**
- ✅ README.md
- ✅ .gitignore (Select Jekyll/Hugo if using static site generator)

**Initial README.md content:**
```markdown
# ABCFarmsIL Documentation

Public documentation for ABCFarmsIL regenerative agricultural infrastructure systems.

## Quick Links

- [Main Project](https://github.com/abcfarmsil/abcfarmsil-core)
- [Algae PBR System](https://github.com/abcfarmsil/abcfarmsil-algae-pbr)
- [Yellow Perch Hatchery](https://github.com/abcfarmsil/abcfarmsil-perch-hatchery)

## Documentation

Coming soon - comprehensive documentation site.

---

© 2026 ABCFarmsIL. All rights reserved.
```

---

## 🔗 Step 5: Link Repositories

### Add Repository Links to READMEs

**In `abcfarmsil-core/README.md`:**
```markdown
## Related Repositories

- **Algae PBR System:** [abcfarmsil/abcfarmsil-algae-pbr](https://github.com/abcfarmsil/abcfarmsil-algae-pbr)
- **Yellow Perch Hatchery:** [abcfarmsil/abcfarmsil-perch-hatchery](https://github.com/abcfarmsil/abcfarmsil-perch-hatchery)
- **Documentation:** [abcfarmsil/abcfarmsil-docs](https://github.com/abcfarmsil/abcfarmsil-docs)
```

**In system-specific READMEs:**
```markdown
## Related Repositories

- **Main Project:** [abcfarmsil/abcfarmsil-core](https://github.com/abcfarmsil/abcfarmsil-core)
- **Documentation:** [abcfarmsil/abcfarmsil-docs](https://github.com/abcfarmsil/abcfarmsil-docs)
```

---

## 🛠️ Step 6: Configure Repository Settings

### For Each Repository:

1. **Go to Settings → General**
   - Update repository name and description if needed
   - Set repository URL
   - Delete branch on merge: Enable
   - Allow squash merging: Enable
   - Allow rebase merging: Disable (keep history clean)
   - Allow merge commits: Disable

2. **Go to Settings → Branches**
   - Add branch protection rule for `main` branch
   - Require pull request reviews: Enable
   - Require status checks to pass: Enable (when tests added)
   - Require branches to be up to date: Enable

3. **Go to Settings → Options**
   - Enable issues
   - Enable discussions
   - Enable wikis
   - Set repository topics (see below)

### Repository Topics (Tags)

**For abcfarmsil-core:**
```
agriculture, aquaculture, microgreens, controlled-environment-agriculture, cea, vertical-farming, hydroponics, sustainable-agriculture, regenerative-agriculture, infrastructure, water-management
```

**For abcfarmsil-algae-pbr:**
```
algae, photobioreactor, pbr, microalgae, food-production, nutraceuticals, culinary-algae, controlled-environment, container-farming
```

**For abcfarmsil-perch-hatchery:**
```
aquaculture, fish-hatchery, yellow-perch, recirculating-aquaculture-system, ras, fish-farming, sustainable-aquaculture, container-aquaculture
```

---

## 🎨 Step 7: Add README Badges (Optional)

### Add to Repository READMEs

```markdown
![License](https://img.shields.io/badge/license-Copyright%202026%20ABCFarmsIL-blue)
![Status](https://img.shields.io/badge/status-In%20Development-yellow)
![GitHub](https://img.shields.io/badge/GitHub-ABCFarmsIL-black)
```

---

## 📊 Step 8: Create Project Boards (Optional)

### Create Projects for Tracking

1. **Go to Projects tab**
2. Click "New project"
3. Choose board template
4. Create projects for:
   - Architecture & Design
   - Algae PBR Development
   - Perch Hatchery Development
   - Documentation
   - Research & Development

### Sample Columns
- Backlog
- To Do
- In Progress
- Review
- Done

---

## 🔒 Step 9: Security Settings

### Enable Security Features

1. **Go to Settings → Security**
2. Enable Dependabot alerts
3. Enable Dependabot security updates (when code added)
4. Configure security policies
5. Add CODEOWNERS file for review assignments

### Create CODEOWNERS file

```# In each repository root directory
# Core Team
* @abcfarmsil/admin @abcfarmsil/lead-developer

# Documentation
/docs/* @abcfarmsil/documentation-team

# Algae PBR Specific
/algae-pbr/* @abcfarmsil/algae-team

# Hatchery Specific
/hatchery/* @abcfarmsil/aquaculture-team
```

---

## 📧 Step 10: Set Up Notifications

### Configure Email Notifications

1. **Go to Settings → Notifications**
2. Choose notification preferences
3. Set watching/ignoring for repositories
4. Configure email frequency

---

## ✅ Step 11: Initial Commit Checklist

Before pushing initial commits:

- [ ] All README files created and populated
- [ ] CONTRIBUTING.md added to core repository
- [ ] License file added to each repository
- [ ] Repository topics/tags configured
- [ ] Repository settings configured
- [ ] Branch protection rules enabled
- [ ] Initial issues created (if desired)
- [ ] Repository descriptions updated
- [ ] Cross-repository links verified

---

## 🚀 Step 12: First Push

### Using Git Command Line

```bash
# Clone repository
git clone https://github.com/abcfarmsil/abcfarmsil-core.git
cd abcfarmsil-core

# Add files
git add README.md CONTRIBUTING.md docs/

# Commit
git commit -m "Initial commit - Core repository setup"

# Push
git push origin main
```

### Using GitHub Web Interface

1. Go to repository page
2. Click "Upload files"
3. Drag and drop files
4. Add commit message
5. Click "Commit changes"

---

## 📋 Step 13: Create Initial Issues (Optional)

Create issues to organize work:

**Example Issues:**
1. [Documentation] Create architecture diagrams
2. [Algae PBR] Detailed PBR panel specifications
3. [Hatchery] Supplier research for Illinois market
4. [Research] Literature review on yellow perch hatchery practices
5. [Business] Partnership outreach list

---

## 🎯 Next Steps

### Immediate (Week 1)
- Set up all repositories
- Create README files
- Configure repository settings
- Add initial documentation

### Short-term (Month 1)
- Add system diagrams
- Create detailed specifications
- Set up project boards
- Start issue tracking

### Medium-term (Quarter 1)
- Complete documentation hierarchy
- Add code for control systems
- Create testing procedures
- Establish workflow processes

### Long-term (Year 1)
- Comprehensive documentation site
- Active community engagement
- Partnership integrations
- Production deployment guides

---

## 📞 Need Help?

If you encounter issues during setup:
- Review [GitHub Documentation](https://docs.github.com)
- Check existing repositories for examples
- Contact the ABCFarmsIL team for guidance

---

## 📄 License

© 2026 ABCFarmsIL. All rights reserved.