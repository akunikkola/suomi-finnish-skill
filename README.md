# Suomi Finnish Skill for Claude Code

**Teach Claude to write correct Finnish.** This skill gives Claude Code comprehensive Finnish language rules — spelling, grammar, punctuation, compound words, and style — so it produces natural, publication-ready Finnish instead of the awkward, anglicism-filled output LLMs typically generate.

Built on the official [Kielitoimiston ohjepankki](https://kielitoimistonohjepankki.fi/) (Institute for the Languages of Finland).

---

## Why this exists

LLMs make predictable mistakes when writing Finnish:

- **Compound words split apart**: "verkko sivusto" instead of *verkkosivu*, "asiakas palvelu" instead of *asiakaspalvelu*
- **Anglicisms everywhere**: "sukella syvemmalle", "implementoida", "adressoida"
- **Wrong punctuation**: English-style decimals (3.14 instead of 3,14), Oxford commas, missing commas before subordinate clauses
- **Overly pompous tone**: American corporate rhetoric translated literally into Finnish
- **Capitalization errors**: weekdays, months, and nationalities capitalized (English rules applied to Finnish)

This skill catches and prevents all of these. It's been used in production to generate hundreds of pages of Finnish web content.

## Installation

### Option 1: Add to a project (recommended)

Copy the `SKILL.md` file into your project's Claude Code skills directory:

```bash
# Create the skills directory if it doesn't exist
mkdir -p .claude/skills

# Copy the skill
cp SKILL.md .claude/skills/suomi-finnish.md
```

The skill will automatically activate when Claude Code detects Finnish language work.

### Option 2: Add globally (all projects)

```bash
# Create the global skills directory if it doesn't exist
mkdir -p ~/.claude/skills

# Copy the skill
cp SKILL.md ~/.claude/skills/suomi-finnish.md
```

### Option 3: One-liner install from GitHub

```bash
# Project-level
mkdir -p .claude/skills && curl -sL https://raw.githubusercontent.com/akunikkola/suomi-finnish-skill/main/SKILL.md -o .claude/skills/suomi-finnish.md

# Global
mkdir -p ~/.claude/skills && curl -sL https://raw.githubusercontent.com/akunikkola/suomi-finnish-skill/main/SKILL.md -o ~/.claude/skills/suomi-finnish.md
```

## What it covers

| Area | Examples |
|---|---|
| Compound words | When to join vs. separate, hyphenation rules |
| Punctuation | Comma rules, decimal comma, no Oxford comma |
| Capitalization | Lowercase weekdays, months, nationalities |
| Numbers & units | Space as thousands separator, unit spacing (5 kg, 15 %) |
| Abbreviations | Dot rules, inflection with colons (EU:n) |
| Dashes | Hyphen (-) vs. en dash (--) usage |
| Sentence structure | Case agreement, postpositions, possessive suffixes |
| AI-specific errors | Anglicisms, overly formal tone, filler text |
| Proofreading | 6-step review checklist |

## Usage

Once installed, the skill activates automatically when you:

- Write or generate Finnish text
- Proofread or review Finnish content
- Translate content into Finnish
- Create content for Finnish websites or services

You can also invoke it manually:

```
/suomi-finnish
```

## Sources

All rules are based on:

- [Kielitoimiston ohjepankki](https://kielitoimistonohjepankki.fi/) (Institute for the Languages of Finland)
- [Kielitoimiston sanakirja](https://www.kielitoimistonsanakirja.fi/) (Dictionary of Contemporary Finnish)
- [Iso suomen kielioppi](https://kaino.kotus.fi/visk/etusivu.php) (Comprehensive Finnish Grammar)

## Contributing

Found a rule that's missing or incorrect? Open an issue or PR. Finnish language nerds welcome.

## License

MIT

---

# Suomi Finnish Skill Claude Codelle

**Opeta Claude kirjoittamaan oikeaa suomea.** Tämä skill antaa Claude Codelle kattavat suomen kielen säännöt — oikeinkirjoituksen, kieliopin, pilkutuksen, yhdyssanat ja tyylin — jotta se tuottaa luonnollista, julkaisukelpoista suomea anglismien täyttämän konekielen sijaan.

Perustuu [Kielitoimiston ohjepankin](https://kielitoimistonohjepankki.fi/) virallisiin ohjeisiin.

## Asennus

### Vaihtoehto 1: Projektitasoinen asennus (suositeltu)

```bash
mkdir -p .claude/skills
cp SKILL.md .claude/skills/suomi-finnish.md
```

### Vaihtoehto 2: Globaali asennus (kaikki projektit)

```bash
mkdir -p ~/.claude/skills
cp SKILL.md ~/.claude/skills/suomi-finnish.md
```

### Vaihtoehto 3: Suora asennus GitHubista

```bash
# Projektitasoinen
mkdir -p .claude/skills && curl -sL https://raw.githubusercontent.com/akunikkola/suomi-finnish-skill/main/SKILL.md -o .claude/skills/suomi-finnish.md

# Globaali
mkdir -p ~/.claude/skills && curl -sL https://raw.githubusercontent.com/akunikkola/suomi-finnish-skill/main/SKILL.md -o ~/.claude/skills/suomi-finnish.md
```

## Mitä skill kattaa

- Yhdyssanasäännöt (yleisin virhetyyppi)
- Pilkutus (sivulauseet, päälauseet, luettelot)
- Iso ja pieni alkukirjain
- Numerot, lyhenteet ja mittayksiköt
- Ajatusviiva vs. yhdysviiva
- Lauserakenne ja kielioppi
- Tekoälylle tyypilliset virheet (anglismit, mahtipontisuus, täytesanat)
- 6-vaiheinen oikolukuprosessi

## Lisenssi

MIT
