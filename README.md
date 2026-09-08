# IT Project — Code Name: Grand Warden

**Skill Directory for Modern Web Application & SaaS Development** — Progressive Disclosure Edition.

This repository is a **Skill** optimized for Claude (Code / Claude.ai). Unlike a
single monolithic `SKILL.md`, it uses a small parent file + 6 per-category
reference files, so Claude only reads the content that is actually relevant to
the user's request — saving tokens on every skill invocation.

> **Scope:** modern web & SaaS applications (2024–2026): React/Vue/Next.js,
> Node.js/FastAPI/Go/Spring Boot, PostgreSQL/MongoDB/Redis, Docker/Kubernetes,
> AWS/GCP/Azure, observability, PWA, microservices.
> For native desktop projects, see the sister repository `it-project-codename-royalchampion`.

## Repository Structure

```javascript
it-project-codename-grandwarden/
├── SKILL.md                 # compact routing file (always loaded first)
└── reference/
    ├── technical.md           # Software Architect, Lead Developer, Front-End, Back-End
    ├── project-management.md  # Project Manager, Scrum Master
    ├── design.md              # UX Designer, UI Designer, UX Researcher
    ├── testing.md             # QA Engineer (Manual), QA Automation, Security Tester
    ├── infrastructure.md      # DevOps Engineer, SysAdmin, Release Manager
    └── strategy.md            # Product Manager, Product Owner
```

17 roles across 6 categories, covering the full SDLC of a modern web/SaaS
application: strategy, design, development, testing & security, deployment &
infrastructure, and project management.

## How It Saves Tokens

- The frontmatter `description` is kept short but still contains all trigger keywords.
- `SKILL.md` contains a **routing table** — Claude knows exactly which single
file to open for a given request.
- Detailed role descriptions live in `reference/*.md` and are only read on demand.
- No duplicated content across files.

## How to Use

### Option 1 — Claude Code (recommended)

```powershell
# from your project folder (Windows)
git clone https://github.com/ifredrix/it-project-codename-grandwarden.git
xcopy /E /I "it-project-codename-grandwarden" ".claude\skills\grandwarden"
```

Claude Code automatically loads `SKILL.md` and only opens `reference/*.md`
when needed.

### Option 2 — Claude.ai (web)

1. Go to **Settings → Capabilities → Skills** (or upload via chat, depending on your plan).
2. Upload `SKILL.md` as the skill definition.
3. When Claude needs details on a role, attach only the single relevant file
from `reference/` — not the whole folder.

## Contributing

If you find roles or skills that are less relevant to modern web development,
or wish to add new trending technologies, feel free to open an **issue** or
submit a **pull request**.

## License

MIT — see [LICENSE](LICENSE).

## Donate

Like this skill? Support me (Bitcoin): **1HZ2h3yyYULFT4jEGwB5ESAZUhBj7kPUa2**

---

> *"Guard the web. Scale the future."*
