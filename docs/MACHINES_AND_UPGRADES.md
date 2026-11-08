# Machines and Upgrades

There are currently exactly three machines.

## 1. Molecular Microscope

**Purpose:** Analyze the current case and reveal its attributes.

- No player upgrade path.
- Its capabilities progress automatically with the campaign phase.
- Phase I reveals Family I.
- Phase II introduces Family II.
- Phase III introduces Family III.
- The final case reveals its Family IV attribute.

The microscope should not conceal information arbitrarily. Its limits are based on campaign progression, not on an upgrade grind.

## 2. Molecular Fabricator

**Purpose:** Combine compounds and fabricate copies of previously discovered compounds.

The Molecular Fabricator combines the responsibilities of the earlier Molecular Workstation and Substance Fabricator concepts.

### Compound synthesis

- The player combines two existing compounds to attempt to create a new compound.
- A successful synthesis creates a compound whose molecule set is the union of the input molecule sets.
- Duplicate molecule IDs are deduplicated.
- A successful synthesis permanently registers the resulting compound's blueprint in the catalogue.
- A failed synthesis consumes both input compounds.

### Fabrication

- The player can duplicate only compounds whose blueprints have already been discovered and registered.
- Fabrication costs energy.
- Energy regenerates passively.
- The Fabricator's upgrade improves **energy regeneration only**.

Whether synthesis itself costs energy, and whether synthesis has a success probability, still need a final decision. Do not assume that the Fabricator upgrade improves synthesis success; the latest agreed upgrade direction is energy regeneration only.

## 3. Bioassay Simulator

**Purpose:** Submit and test a candidate cure against the current case.

- Compares the submitted molecule set with the required molecule set.
- Returns success or failure according to the exact-match rule.
- Its only upgrade improves operating speed / reduces simulation time.
- No upgrade to simultaneous test capacity is planned.

The simulator's failure feedback should be useful without necessarily revealing the exact missing or extra molecule. The feedback model remains to be designed.

## Upgrade economy

- One currency: money.
- A centralized upgrade interface is used.
- The player presses one upgrade action to upgrade all applicable machines together.
- No separate currency or individual upgrade menu for each machine.

| Machine | Upgrade behavior |
|---|---|
| Molecular Microscope | No upgrade; follows campaign phase |
| Molecular Fabricator | Increases energy regeneration |
| Bioassay Simulator | Reduces simulation time |

Energy storage capacity is currently assumed to remain fixed unless the design is deliberately changed later.
