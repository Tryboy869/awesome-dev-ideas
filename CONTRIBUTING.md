# Contributing to /dev/ideas

Thank you for your interest in contributing! This document explains how to submit ideas, what makes a good submission, and the review process.

---

## 📋 Quick Start

**Submitting an idea takes 4 steps:**

1. **Fork** this repository
2. **Create** a JSON file in `ideas/your-idea-slug.json`
3. **Follow** the structure defined in [`schema/idea.schema.json`](schema/idea.schema.json)
4. **Open** a Pull Request

**Our automated validation will check your submission**, and a maintainer will review the content.

---

## ✅ What Makes a Good Idea?

### Core Principle
> **"Any idea is valid as long as it's coherent."**

An idea doesn't need to be:
- ✗ Already implemented
- ✗ Commercially viable
- ✗ Academically rigorous

But it **must** have:
- ✓ A clear technical problem
- ✓ An identifiable approach or intuition
- ✓ Proof it's not nonsense (constraints, edge cases, or prior art)

---

## 📝 JSON Structure

### Required Fields

```json
{
  "id": "unique-slug-here",
  "title": "Concise Title of Your Idea",
  "category": "distributed-systems",
  "status": "hypothesis",
  "author": {
    "github": "your-username",
    "doi": null
  },
  "content": {
    "problem": "What technical problem does this solve? (20-500 chars)",
    "approach": "High-level intuition or method (20-500 chars)",
    "why_not_bullshit": "Why this is technically coherent (20-500 chars)"
  },
  "metadata": {
    "created": "2026-01-24",
    "updated": "2026-01-24",
    "tags": ["tag1", "tag2", "tag3"]
  }
}
```

### Optional: Proofs (required for `poc` or `validated` status)

If your idea has reached **PoC** or **Validated** stage, you **must** include proof:

```json
{
  ...
  "status": "poc",
  "proofs": [
    {
      "type": "github",
      "url": "https://github.com/user/repo",
      "description": "Working prototype with benchmarks"
    },
    {
      "type": "video",
      "url": "https://youtube.com/watch?v=...",
      "description": "5-minute demo walkthrough"
    }
  ]
}
```

**Accepted proof types:**
- `github` / `gitlab` — Source code
- `colab` / `jupyter` — Interactive notebooks
- `video` — YouTube, Vimeo, Loom (3-10 min demos)
- `demo` — Live sites (Vercel, Netlify, etc.)
- `paper` — arXiv, DOI, or hosted PDF

**Limit: 3 proofs maximum**

---

## 🔄 Idea Lifecycle

Your idea will evolve through these stages:

| Status | Description | Requirements |
|--------|-------------|--------------|
| **hypothesis** | Untested intuition | Just the 3 core content fields |
| **experimentation** | Active testing | Mention experimental data in `why_not_bullshit` |
| **concept** | Structured approach | Document architecture or design |
| **poc** | Working prototype | **At least 1 proof required** |
| **validated** | Reproduced by others | **Multiple implementations cited** |

You can update your idea's status by submitting a new PR that modifies your JSON file.

---

## 🎯 Categories

Choose the **primary** category that best fits your idea:

- `distributed-systems`
- `ai`
- `programming-languages`
- `developer-tools`
- `security`
- `networking`
- `databases`
- `hardware`
- `meta-programming`
- `other`

---

## 🚀 Submission Process

### Step 1: Create Your JSON File

```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/ideas.git
cd ideas

# Create your idea file
cp ideas/distributed-sqlite-crdt.json ideas/my-awesome-idea.json

# Edit it with your content
nano ideas/my-awesome-idea.json
```

### Step 2: Validate Locally (Optional)

```bash
# Install ajv-cli
npm install -g ajv-cli ajv-formats

# Validate your JSON
ajv validate -s schema/idea.schema.json -d ideas/my-awesome-idea.json
```

### Step 3: Open a Pull Request

```bash
git add ideas/my-awesome-idea.json
git commit -m "feat: add idea for [Your Title]"
git push origin main
```

Then open a PR on GitHub. Our automated checks will run.

---

## 🤖 Automated Validation

When you open a PR, GitHub Actions will:

1. ✅ Validate JSON structure against the schema
2. ✅ Check for duplicate IDs
3. ✅ Verify that `poc`/`validated` status has proofs
4. ✅ Auto-label your PR if all checks pass

If validation fails, check the error messages and update your PR.

---

## 👥 Review Process

**After automated validation:**

1. A maintainer will review your idea's **content** (not just structure)
2. They may ask questions or suggest improvements via PR comments
3. Once approved, your PR will be merged
4. **A GitHub Discussion will be created automatically** for your idea

---

## 📜 Code of Conduct

We enforce a strict **zero-tolerance policy** for:

- ❌ Personal attacks or harassment
- ❌ Dismissive or toxic comments
- ❌ Trolling or bad-faith arguments

**Violators will be warned once, then banned.**

### Our Standard

- ✅ Critique **ideas**, never **people**
- ✅ Assume good faith
- ✅ Be constructive and kind

---

## 🎓 Academic Attribution

If you want your idea to be citable:

1. Upload your idea document to [Zenodo](https://zenodo.org) or [HAL](https://hal.science)
2. Get a DOI
3. Add it to your idea's `author.doi` field

Ideas with DOIs will receive a 🎓 badge on the website.

---

## 🔗 Linking to Discussions

Once your idea is merged, a GitHub Discussion will be created. You can:

- Share the discussion URL on social media
- Link to it in blog posts or papers
- Invite collaborators to discuss there

---

## 🙋 Need Help?

- **Questions about submission?** [Open a Discussion](https://github.com/Tryboy869/ideas/discussions)
- **Found a bug in the website or automation?** [Open an Issue](https://github.com/Tryboy869/ideas/issues)
- **Want to become a maintainer?** Contribute consistently for 3+ months, then reach out to [@anzize](https://github.com/anzize)

---

**Thank you for contributing to /dev/ideas!** 🚀