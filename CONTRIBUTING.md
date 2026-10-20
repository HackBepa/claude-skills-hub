# 🤝 Contributing to Claude Skills Hub

Thanks for your interest in improving this hub! Every skill here aims to be **tested, documented, and ready to use by anyone** — no personal data, no hidden dependencies.

---

## 💡 Ways to Contribute

| Type | How |
| :--- | :--- |
| 🐛 **Report a bug** | Open an Issue describing the prompt you used, what you expected, and what Claude actually did. |
| ✨ **Suggest an improvement** | Open an Issue with the `enhancement` label before starting big changes, so we can discuss it first. |
| 🛠️ **Improve an existing skill** | Fork the repo, make your change, and open a Pull Request. |
| 🚀 **Propose a new skill** | Open an Issue with a short pitch: what problem it solves and who it's for. |

---

## 📂 Skill Structure

Every skill lives in its own folder inside `skills/`:

```
skills/
└── your-skill-name/
    ├── SKILL.md        # Required: frontmatter + instructions
    ├── README.md       # Required: what it does, commands, install
    └── references/     # Optional: templates or long docs loaded on demand
```

Logos and images go in `assets/`, named after the skill (e.g. `assets/your-skill-name-logo.png`).

### Required frontmatter

```yaml
---
name: your-skill-name
description: What the skill does AND when Claude should use it. Be specific about trigger phrases and contexts.
---
```

The `description` is how Claude decides when to load the skill, so it deserves as much care as the instructions themselves.

---

## ✅ Quality Rules

1. **Test before you submit.** Run the skill in Claude with at least 2–3 real prompts. In your PR, describe what you tested and what the output looked like.
2. **No personal or private data.** Skills must work for anyone out of the box: no names, emails, API keys, internal URLs, or company-specific content.
3. **No copyrighted material.** Don't include course PDFs, paid material, or notes generated from them — not in the skill, the examples, or the screenshots. Use public sources (official docs, OWASP, open textbooks) for demos.
4. **No destructive actions without confirmation.** If a skill writes, overwrites, or deletes files, it must ask the user first.
5. **Respect the source.** Skills that process documents must not invent facts that aren't in the input.
6. **Keep the identity.** Banners, personas, and visual style are welcome, as long as they don't break the skill's behavior.

---

## 🔀 Pull Request Process

1. Fork the repo and create a branch: `feat/skill-name-change` or `fix/skill-name-bug`.
2. Make your changes, keeping each PR focused on **one skill and one change**.
3. If you change behavior or commands, update that skill's `README.md`.
4. Open the PR using this checklist:

```markdown
- [ ] Tested in Claude (claude.ai and/or Claude Code)
- [ ] Prompts tested and results described below
- [ ] No personal data or copyrighted material
- [ ] Frontmatter has `name` and `description`
- [ ] README updated (if behavior changed)
```

Maintainers will review, may suggest changes, and merge once it's ready.

---

## 📝 Commit Style

Short, descriptive, in English:

```
feat(cert-master): add collapsible answers to /quiz
fix(cert-master): banner repeating on every response
docs: update installation steps
```

---

## 💬 Code of Conduct

Be respectful and constructive. Critique the skill, not the person. Everyone here is learning.

---

## ⚖️ License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE) of this repository.