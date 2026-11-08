# Core Gameplay Loop

## Intended loop

1. **Receive a case.** Lucien assigns the next research case and frames it as a medical problem.
2. **Analyze the sample.** The Molecular Microscope reveals the attributes available at the current campaign phase.
3. **Research unknown interactions.** The player experiments to discover which fictional molecules counteract which attributes.
4. **Create or obtain compounds.** The player uses the Molecular Fabricator to combine or duplicate discovered compounds.
5. **Submit a candidate cure.** The player sends the molecule set to the Bioassay Simulator.
6. **Review the result.** The simulator reports whether the submitted set is an exact match.
7. **Progress.** A successful treatment advances the campaign to the next case.

## Research and discovery

The player must discover the counteracting molecule for each attribute. There is no in-game table that simply lists the answers.

The first three families are not automatically solved for the player; their solutions are also learned through experimentation. Family IV is especially difficult.

The exact experiment interface and feedback rules have not yet been finalized. The system should be understandable and fair:
- Experiments should produce useful information.
- Failed attempts should not create an unwinnable state.
- The player should be able to record or revisit discoveries.
- The final family should be challenging without becoming an arbitrary combinatorial grind.

## Exact-match cure rule

A candidate cure succeeds only when its molecule set is identical to the required molecule set.

- Missing molecule: failure.
- Extra molecule: failure.
- Correct molecules in a different order: success.
- Duplicate entries: treated as one molecule, not as additional quantities.

## Scope guardrails

Do not add extra simulation layers unless they materially improve the core loop. Numerical attribute strengths, real chemistry, temperature/pressure simulation, compound durability, multiple currencies, and large resource trees are not part of the current design.
