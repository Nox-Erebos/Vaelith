# Vaelith

A finite, narrative-driven sci-fi laboratory game about research, discovery, and the consequences of work done in good faith.

> **Core premise:** The player believes she is developing cures to help people. In reality, the compounds she creates are being used by her nation's military to dismantle the immune defenses of an ancient alien species: the Vaelith.

This repository is the current game-design reference. It is intentionally written as Markdown so it can be committed to GitHub and revised as the project develops.

## Design pillars

- **A focused solo-developer scope.** Keep systems implementable and avoid unnecessary simulation complexity.
- **Research through experimentation.** The player discovers how fictional molecules interact with attributes; no solution table is handed to them.
- **A finite campaign.** Ten cases, three phases, one final case, and a deliberate ending.
- **A quiet moral reveal.** The protagonist is compassionate and sincere. The horror comes from what her work was used to accomplish.
- **Ancient, mysterious science fiction.** The Vaelith should feel like an old and unfamiliar form of life, not generic monsters.

## Current canon at a glance

| Element | Current decision |
|---|---|
| Game title / species name | **Vaelith** |
| Protagonist | **Dr. Elara Voss**, female researcher |
| Commander | **Dr. Lucien Veyr** |
| Alien witness | A Vaelith woman who remains **unnamed** |
| Campaign | 10 cases: 3 + 3 + 3 + 1 |
| Attribute families | 4 |
| Attributes in Families I–III | 3 per family |
| Family IV | 5 possible attributes; final case has 1 |
| Attribute values | None; attributes are present or absent |
| Cure rule | Exact molecule-set match |
| Machines | Molecular Microscope, Molecular Fabricator, Bioassay Simulator |
| Ending | The military purpose of the research is revealed |

## Repository map

- [`docs/LORE.md`](docs/LORE.md) — premise, Vaelith, and military deception
- [`docs/CHARACTERS.md`](docs/CHARACTERS.md) — Elara, Lucien, and the unnamed witness
- [`docs/CAMPAIGN.md`](docs/CAMPAIGN.md) — the ten-case structure
- [**Attributes & Molecules**](docs/Attributes-&-Molecules.md) — all attribute families and proposed counteracting molecules
- [`docs/GAMEPLAY_LOOP.md`](docs/GAMEPLAY_LOOP.md) — research, synthesis, testing, and progression
- [`docs/MACHINES_AND_UPGRADES.md`](docs/MACHINES_AND_UPGRADES.md) — machine responsibilities and upgrade rules
- [`docs/SAVE_DATA.md`](docs/SAVE_DATA.md) — compound inventory, catalogue, and research knowledge
- [`docs/ENDING_AND_RECORDING.md`](docs/ENDING_AND_RECORDING.md) — final reveal and recording concept
- [`docs/OPEN_QUESTIONS.md`](docs/OPEN_QUESTIONS.md) — decisions that are not settled yet

## Status and terminology

Names for the attribute families, attributes, compounds, and individual Vaelith immune cells are **working proposals**, not locked canon. The character names and the woman's nameless status are the current selected direction. Where a rule has not been confirmed, the docs label it as proposed or unresolved rather than treating it as final.

All chemistry and biological mechanisms are fictional abstractions. They are not intended to model real pathogens or provide real-world biological procedures.
