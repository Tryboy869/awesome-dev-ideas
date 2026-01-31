<p align="center">
  <img src=".github/assets/hero-animation.svg" width="600" alt="/dev/ideas animated logo"/>
</p>

<p align="center">
  <strong>The open registry for proof-of-concept technical ideas</strong>
</p>

<p align="center">
  <a href="https://tryboy869.github.io/dev-ideas/"><img src="https://img.shields.io/badge/catalog-live-brightgreen" alt="Website"></a>
  <a href="https://tryboy869.github.io/dev-ideas/ideas.json"><img src="https://img.shields.io/badge/dynamic/json?url=https://tryboy869.github.io/dev-ideas/ideas.json&query=$.length&label=ideas&color=blue" alt="Ideas Count"></a>
  <a href="CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
  <a href="LICENSE.md"><img src="https://img.shields.io/badge/License-CC%20BY--SA%204.0-blue.svg" alt="License"></a>
  <a href="https://github.com/Tryboy869/dev-ideas/discussions"><img src="https://img.shields.io/github/discussions/Tryboy869/dev-ideas" alt="GitHub Discussions"></a>
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
</p>

<p align="center">
  <strong>Founded by <a href="https://github.com/anzize">Daouda Abdoul Anzize</a> — January 2026</strong>
</p>

Computational Paradigm Designer • 40+ open-source projects  
[Portfolio](https://tryboy869.github.io/daa) • [Twitter/X](https://twitter.com/Nexusstudio100) • [LinkedIn](https://linkedin.com/in/anzize-adéléké-daouda)

---

## ⚡ Quick Start (30 seconds)

```bash
# Browse existing ideas
open https://tryboy869.github.io/dev-ideas/

# Submit your idea
git clone https://github.com/Tryboy869/dev-ideas.git
cp template.json ideas/my-idea-slug.json
# Edit ideas/my-idea-slug.json with your concept
git add . && git commit -m "feat: add my-idea-slug" && git push
```

**[Visual Catalog →](https://tryboy869.github.io/dev-ideas/)** • **[Contribution Guide →](CONTRIBUTING.md)**

---

## 🎯 Why This Exists

**The problem**: You have a technical idea. Where do you put it?

- ❌ **Academic papers** → 6+ months review, paywalls
- ❌ **GitHub repos without context** → invisible, no validation
- ❌ **Twitter threads** → ephemeral, lost in noise
- ❌ **Private notes** → never validated, never built

**The solution**: A structured, searchable registry where:
- ✅ Ideas evolve from **Hypothesis → PoC → Validated**
- ✅ Community validates via **GitHub Discussions**
- ✅ Proper attribution (**CC BY-SA 4.0**)
- ✅ Discoverable by **search engines + LLMs**

**Real-world use cases**:
- 🔬 **Researcher** wants to test hypothesis before committing to full paper
- 💡 **Developer** has 3 side project ideas, wants community feedback on which to pursue
- 🛠️ **Team** needs to document R&D explorations for future reference
- 🌐 **Open-source maintainer** wants to crowdsource feature ideas

---

## 🚀 How It Works

```
1. Submit → JSON file via Pull Request
2. Validate → Automated structure check
3. Discuss → GitHub Discussion opens automatically
4. Evolve → Hypothesis → Experimentation → Concept → PoC → Validated
```

**Your idea. Our collective validation.**

---

## 📊 Current Status

- 🌱 **Just launched** (January 2026)
- 💡 10 seed ideas to demonstrate format
- 🔨 Actively seeking contributors

**[Explore the catalog →](https://tryboy869.github.io/ideas/)**

---

## 🛠️ Idea Lifecycle

<!--lint disable table-pipe-alignment-->
| Phase               | Description                     | Example                                        |
| --------------------- | --------------------------------- | ------------------------------------------------ |
| **Hypothesis**      | Untested intuition              | "What if SQLite used CRDTs?"                   |
| **Experimentation** | Active testing, collecting data | "Built a basic prototype, seeing 20% overhead" |
| **Concept**         | Structured approach             | "CRDT layer design documented"                 |
| **PoC**             | Working prototype               | "Demo repo with benchmarks"                    |
| **Validated**       | Reproduced by others            | "3+ independent implementations"               |

<!--lint enable table-pipe-alignment-->
---

## 📝 How to Contribute


**Quick start:**
1. Fork this repo
2. Create `ideas/your-idea-slug.json` following the [schema](schema/idea.schema.json)
3. Open a Pull Request
4. Automated validation runs
5. If approved, a Discussion thread is created automatically

---

## 📂 Repository Structure

```
/dev/ideas/
├── .github/
│   └── workflows/
│       ├── validate-idea.yml      # Validates JSON structure
│       ├── create-discussion.yml  # Auto-creates GitHub Discussion
│       └── build-site.yml         # Generates static site
├── ideas/
│   ├── distributed-sqlite-crdt.json
│   ├── neural-kernel-scheduler.json
│   └── ...
├── schema/
│   └── idea.schema.json           # JSON Schema for validation
├── docs/
│   ├── index.html                 # Generated website
│   └── ideas.json                 # Auto-generated from ideas/*.json
├── README.md                       # English docs
├── README_FR.md                    # French docs
├── CONTRIBUTING.md                 # English contribution guide
├── CONTRIBUTING_FR.md              # French contribution guide
├── LICENSE.md
└── CODE_OF_CONDUCT.md
```

---

## 🔥 Featured Ideas

<!--lint disable awesome-list-item double-link-->

### Recently Validated
- **[Neural Kernel Scheduler](ideas/neural-kernel-scheduler.json)** <img src="docs/badges/validated.svg" height="20" alt="Validated"> — 3 independent implementations confirmed 20% latency improvement

### Active Experimentation  
- **[Self-Healing WebAssembly](ideas/self-healing-wasm.json)** <img src="docs/badges/experimentation.svg" height="20" alt="Experimentation"> — 2 teams testing automatic rollback mechanisms

### New Hypotheses
- **[Distributed SQLite CRDT](ideas/distributed-sqlite-crdt.json)** <img src="docs/badges/hypothesis.svg" height="20" alt="Hypothesis"> — Looking for experimenters to test overhead impact


---

<!--lint enable awesome-list-item double-link-->

## 🤝 Governance

<!--lint disable awesome-list-item double-link-->

- **Founding Maintainer**: [Daouda A. Anzize](https://github.com/anzize)
- **License**: CC BY-SA 4.0 (ideas), MIT (code/scripts)
- **Decisions**: Community consensus via Discussions
- **Maintainer Rotation**: New co-maintainers every 6 months

**This is a community project.** The founder's role is to curate, not control.

---

<!--lint enable awesome-list-item double-link-->

## 📜 License

<!--lint disable awesome-list-item double-link-->

- **Ideas, descriptions, documentation**: [CC BY-SA 4.0](LICENSE.md)
- **Code snippets, scripts**: [MIT](LICENSE.md)

---

<!--lint enable awesome-list-item double-link-->

## 🌟 Recognition

If you use an idea from this registry in your work:
- **Academic citation**: Use the provided DOI (if available)
- **Informal attribution**: Link back to the idea's Discussion thread
- **Star this repo** to show support

---

## 📬 Contact

**Questions? Suggestions?**
- Open a [Discussion](https://github.com/Tryboy869/ideas/discussions)
- Email: contact@proton.me

---

**Built with ❤️ by the technical community.**
