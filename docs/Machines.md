# Machines

## 1. Molecular Microscope

**Purpose:** Analyze the current case and reveal its attributes.

- No player upgrade path.
- Its capabilities progress automatically with the campaign phase.
- Reveals all attributes belonging to the "disease"

## 2. Molecular Fabricator

**Purpose:** Combine compounds and fabricate copies of previously discovered compounds.

The Molecular Fabricator combines the responsibilities of the earlier Molecular Workstation and Substance Fabricator concepts.

### Compound synthesis

- The player combines two existing compounds to attempt to create a new compound.
- A successful synthesis creates a compound whose molecule set is the union of the input molecule sets.
- A failed synthesis consumes both input compounds and the energy required to produce them.

### Fabrication

- Fabrication costs energy.
- Energy regenerates passively.
- The Fabricator's upgrade improves **energy regeneration only**.

## 3. Bioassay Simulator

**Purpose:** Submit and test a candidate cure against the current case.

- Compares the submitted molecule set with the required molecule set.
- Returns success or failure according to the exact-match rule.
- Its only upgrade improves operating speed.

## 4. Research Dossier

**Purpose:** Receive details regarding the "disease"

- Gives the player a disease that they have to analyze using the Molecular Microscope.
- Not upgradeable.

## Upgrade economy

- One currency: money.
- Generalized upgrade system: the player presses upgrade; all upgradeable machines upgrade themselves in accordance with predefined parameters.

**Energy:** Energy is consumed by the Fabricator and Simulator. The amount of energy they can hold is fixed.
