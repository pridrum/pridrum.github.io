# This site: Priscila de Azevedo Drummond

Everything below the next horizontal rule is specific to this site and takes precedence over the
upstream al-folio guidance that follows it.

## Voice

The prose on this site is hers. Match it rather than improving it.

- Short declarative sentences, one claim each.
- No em dashes in prose. Use a comma, a colon, or a second sentence. The one exception is a
  verbatim student quote, which is never edited for any reason.
- No bold for emphasis inside prose, and no bolded lead-ins like "**The point first.**"
- Never write that an outcome "cannot be measured". Write hard to quantify, observed indirectly,
  contested, or no single number.
- "Worked in all four analytics modes", never "published across them". The data envelopment
  analysis work is master's theses.
- Participatory operations research is a future direction, not an existing program.
- Name journals, never special issues.
- Banned words: resonates, drawn to, align with.
- Every claim is anchored in a number, a name, a date, or a quote. If the fact is missing, leave it
  missing and ask her. Do not generalize to fill the gap.

## Facts that have been wrong before

These were corrected across several documents at once. Check here before editing any teaching or
CV content, rather than copying from an older page.

- The Teaching Fellowship is Fall 2025 to Spring 2026.
- IE 4516 Quality Assurance ran in Fall 2023, about 20 students. She redesigned the teaching
  materials and taught the design of experiments and process control modules.
- The 3rd and 7th session ranking belongs to IE 5617 Lean, Summer I 2025. It does not belong to
  IE 4516 Quality Assurance. The two are easy to conflate: same instructor, both about 20 students,
  both with a process control module.
- The ANOVA game, The Destruction of Reality Itself, is IE 4516. She designed it and Prof. Hugh
  McManus reviewed it. Never "jointly built" and never "solo".
- The busing case follows a school closing, not a road closure. Road construction in area 6 is a
  sensitivity sub-question.
- Brazil is three and a half years. Never four.
- "Nine years of agency and nonprofit partnership" is retired. Name the organizations instead.
- The scoping review is in preparation for submission to Networks. It is not submitted, whatever
  the CV masters say.

## Local build

Node and Docker are not installed on her machine, and the system Ruby is 2.6 while the lockfile
wants Bundler 4, so `docker compose up`, `bundle exec jekyll serve` and `npx prettier` all fail
locally. Verify changes statically instead: parse the front matter, check permalinks are unique,
and check that every internal link resolves to a permalink or to a file that exists under assets.
CI runs the real build, prettier, and the lychee link check.

---

# Agent Guidelines for al-folio

A simple, clean, and responsive Jekyll theme for academics.

## Quick Links by Role

- **Are you a coding agent?** → Read [`.github/copilot-instructions.md`](.github/copilot-instructions.md) first (tech stack, build, CI/CD, common pitfalls & solutions)
- **Customizing the site?** → See [`.github/agents/customize.agent.md`](.github/agents/customize.agent.md)
- **Writing documentation?** → See [`.github/agents/docs.agent.md`](.github/agents/docs.agent.md)
- **Need setup/deployment help?** → [INSTALL.md](INSTALL.md)
- **Troubleshooting & FAQ?** → [TROUBLESHOOTING.md](TROUBLESHOOTING.md)
- **Customization & theming?** → [CUSTOMIZE.md](CUSTOMIZE.md)
- **Quick 5-min start?** → [QUICKSTART.md](QUICKSTART.md)

## Essential Commands

### Local Development (Docker)

The recommended approach is using Docker.

```bash
# Initial setup & start dev server
docker compose pull && docker compose up
# Site runs at http://localhost:8080

# Rebuild after changing dependencies or Dockerfile
docker compose up --build

# Stop containers and free port 8080
docker compose down
```

### Pre-Commit Checklist

Before every commit, you **must** run these steps:

1.  **Format Code:**
    ```bash
    # (First time only)
    npm install --save-dev prettier @shopify/prettier-plugin-liquid
    # Format all files
    npx prettier . --write
    ```
2.  **Build Locally & Verify:**

    ```bash
    # Rebuild the site
    docker compose up --build

    # Verify by visiting http://localhost:8080.
    # Check navigation, pages, images, and dark mode.
    ```

## Critical Configuration

When modifying `_config.yml`, these **must be updated together**:

- **Personal site:** `url: https://username.github.io` + `baseurl:` (empty)
- **Project site:** `url: https://username.github.io` + `baseurl: /repo-name/`
- **YAML errors:** Quote strings with special characters: `title: "My: Cool Site"`

## Development Workflow

- **Git & Commits:** For commit message format and Git practices, see [.github/GIT_WORKFLOW.md](.github/GIT_WORKFLOW.md).
- **Code-Specific Instructions:** Consult the relevant instruction file for your code type.

| File Type                                     | Instruction File                                                                                |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Markdown content (`_posts/`, `_pages/`, etc.) | [markdown-content.instructions.md](.github/instructions/markdown-content.instructions.md)       |
| YAML config (`_config.yml`, `_data/`)         | [yaml-configuration.instructions.md](.github/instructions/yaml-configuration.instructions.md)   |
| BibTeX (`_bibliography/`)                     | [bibtex-bibliography.instructions.md](.github/instructions/bibtex-bibliography.instructions.md) |
| Liquid templates (`_includes/`, `_layouts/`)  | [liquid-templates.instructions.md](.github/instructions/liquid-templates.instructions.md)       |
| JavaScript (`_scripts/`)                      | [javascript-scripts.instructions.md](.github/instructions/javascript-scripts.instructions.md)   |

## Common Issues

For troubleshooting, see:

- [Common Pitfalls & Workarounds](.github/copilot-instructions.md#common-pitfalls--workarounds) in copilot-instructions.md
- [TROUBLESHOOTING.md](TROUBLESHOOTING.md) for detailed solutions
- [GitHub Issues](https://github.com/alshedivat/al-folio/issues) to search for your specific problem.
