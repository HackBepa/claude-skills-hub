<p align="center">
  <img src="/assets/cert-master-logo.png" width="450" alt="CertMaster OS Logo">
</p>

<p align="center">
  <a href="https://github.com/HackBepa/claude-skills-hub/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue?style=flat-square" alt="License: MIT">
  </a>
  <a href="https://github.com/HackBepa/claude-skills-hub/stargazers">
    <img src="https://img.shields.io/github/stars/HackBepa/claude-skills-hub?style=flat-square&logo=github&label=Give%20a%20star&color=yellow" alt="Give a Star!">
  </a>
</p>

# 📚 CertMaster OS — High-Density Study & Knowledge Architect for Claude

`cert-master` is an elite, production-grade system prompt (Skill) for Anthropic's Claude designed to convert raw, chaotic educational materials (PDFs, official documentation, video transcripts, or lecture notes) into pristine, future-proof **Obsidian** vaults or **Notion** databases.

It implements **progressive disclosure**, **strict anti-hallucination protocols**, and **interactive commands** to supercharge your active recall study workflow.

---

## 🔥 Key Features

- **🧠 Multi-Platform Adaptability:** Natively detects and shapes outputs for **Obsidian** (using YAML frontmatter, internal links `[[Note]]`, and nested callouts) or **Notion** (clean Markdown databases).
- **🛡️ Epistemic Responsibility:** Enforces a zero-extrapolation anchor. If a technical command, flag, or definition isn't explicitly in your source material, Claude will declare ignorance rather than hallucinate.
- **💬 Dual-Response Layer:** Claude acts as an elite mentor in the chat (explaining *why* a concept matters pedagogically) while writing an immaculate technical asset in a single code block for your vault.
- **🧹 Transcription Sanitizer:** Strips out verbal tics, repetitions, and conversational noise from lecture transcripts (YouTube, Udemy) and builds dense academic prose.

---

## 🛠️ Interactive Commands

Once the skill is active, you can trigger these advanced workflows directly in your chat:

| Command | Action | Output Style |
| :--- | :--- | :--- |
| `/setup` | Calibrates the multi-project memory | Interactive onboarding test |
| `/quiz` | Suspends note-taking and launches an active recall test | 5 Exam-style situational questions with hidden answers |
| `/moc` | Compiles an automated Map of Content / Index | Centralized dashboard linked to your generated notes |
| `/video <url>`| Ingests, cleans, and documents video lecture transcripts | Dual pedagogical brief + clean documentation asset |
| `/audit` | Refactors, cleans, and upgrades an existing legacy note | Diagnostic feedback + high-density restructured code |
| `/tools` | Analyzes your tech stack and recommends MCP setups | Verified Model Context Protocol installation guide |

---

## 🚀 Installation & Usage

### Method 1: Claude Web Interface
1. Download the `skills/cert-master` folder from this repository and compress it as a `.zip`.
2. In Claude, go to **Customize > Skills** and upload the `.zip`.
3. Start a new chat and type `/setup` to initialize your tracking profile.

### Method 2: Claude Code (CLI)
Copy the skill folder into your global or local agent skills path:
```bash
cp -r skills/cert-master ~/.claude/skills/
```

---

## 🔌 Supercharge with MCP (Model Context Protocol)

`cert-master` is optimized for **2026 agentic workflows**. Combine this skill with:
- **Filesystem MCP:** To allow Claude to write notes directly into your local Obsidian Vault without copy-pasting.
- **Notion MCP:** To automatically sync generated summaries and quiz blocks straight into your cloud databases via API.

---
MIT License © 2026
