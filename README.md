# RomanEcom Agent Skill

`romanecom` is a portable agent skill for auditing, buying, scaling, and fixing ecommerce brands using the operator playbook Roman Khan described on the What's Working Podcast episode ["How Apple made him $100m | Roman Khan"](https://www.youtube.com/watch?v=PbCr6CttFhA).

It is built for practical work: category calls, acquisition screens, margin repair, supply-chain repair, payment-term float, and distribution-first ecommerce decisions.

It uses the standard `SKILL.md` folder format, so it works with Claude Code, Codex, and other agents that support agent skills.

## What It Does

The skill pushes Codex to evaluate ecommerce brands through:

- Whale and why-now category timing.
- Hero SKU and USP quality.
- PC1, PC2, and PC3 contribution margin math.
- OPEX and revenue per expensive FTE.
- Supply-chain disintermediation.
- Packaging and logistics cost reduction.
- Supplier payment terms, lead times, float, and owner distributions.

The repo does not include the podcast transcript. It includes a paraphrased operating framework with source attribution.

## Install With Skills CLI

Install for your current agent:

```bash
npx skills add Abubakar-Waheed/romanecom-skill --skill romanecom
```

Install for Claude Code explicitly:

```bash
npx skills add Abubakar-Waheed/romanecom-skill --skill romanecom --agent claude-code
```

Install globally for all supported agents on your machine:

```bash
npx skills add Abubakar-Waheed/romanecom-skill --skill romanecom --agent '*' --global --copy
```

Preview/use it without installing:

```bash
npx skills use Abubakar-Waheed/romanecom-skill@romanecom | claude
```

Restart your agent if it does not pick up new skills automatically.

## Manual Install: Claude Code

For a personal Claude Code skill available across projects:

```bash
mkdir -p ~/.claude/skills
cp -R romanecom ~/.claude/skills/romanecom
```

For a project-local Claude Code skill, copy it into your repo:

```bash
mkdir -p .claude/skills
cp -R romanecom .claude/skills/romanecom
```

Then invoke it in Claude Code:

```text
/romanecom audit this ecommerce brand: ...
```

Claude Code can also load it automatically when your request matches the skill description.

## Manual Install: Claude.ai

Claude.ai custom skills are uploaded through the UI:

1. Download or clone this repo.
2. Zip the `romanecom/` folder.
3. In Claude.ai, enable code execution/file creation if needed.
4. Go to `Customize > Skills`.
5. Add a custom skill and upload the zip.
6. Toggle the skill on.

## Manual Install: Codex

Copy the `romanecom/` folder into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
cp -R romanecom ~/.codex/skills/romanecom
```

On Windows PowerShell:

```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\skills" | Out-Null
Copy-Item -Recurse -Force .\romanecom "$env:USERPROFILE\.codex\skills\romanecom"
```

Restart Codex after copying.

## Use

Invoke it explicitly in Codex or another `$skill` style agent:

```text
Use $romanecom to audit this ecommerce brand: ...
```

Invoke it explicitly in Claude Code:

```text
/romanecom audit this ecommerce brand: ...
```

Some clients expose skills through slash commands, chips, or menus. Choose `romanecom` and give it the same task.

## Example Prompts

```text
Use $romanecom to audit a DTC jewelry brand doing $4.2M annual revenue, 62% gross margin, 18% return rate, $82 AOV, $31 CAC, 12 employees, net 30 supplier terms, and 75-day production-to-warehouse lead time.
```

```text
Use $romanecom to screen this acquisition. It is a 9-year-old pet supplements brand at $27M revenue, 14% EBITDA, 70% subscription revenue, net 60 terms, 35-day lead time, and rising search demand for senior dog longevity.
```

```text
Use $romanecom to find the fastest path to owner distributions. Here are my management accounts, supplier terms, inventory position, and marketing spend.
```

More examples live in [`examples/`](examples/).

## Expected Output

The skill defaults to:

- Verdict.
- Scorecard.
- Math.
- Levers.
- Risks.
- Next 30 days.

It is intentionally blunt: revenue is last, owner distributions are first, and advice must tie back to cash, margins, or category timing.
