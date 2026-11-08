# Save Data and Compound Storage

This document describes the logical data the game needs to persist. It is a design reference, not a required serialization format.

## Keep three collections distinct

### 1. Compound inventory

The compounds the player currently owns and can use.

A compound can be consumed during synthesis, so inventory quantity or ownership must be tracked separately from discovery.

### 2. Compound catalogue / blueprints

Every compound the player has successfully discovered.

A blueprint remains registered even if the player later consumes all physical copies of that compound. The player can fabricate another copy if they have the required energy.

### 3. Research knowledge

The attribute-to-molecule relationships the player has experimentally discovered.

This is separate from the compound catalogue. Discovering a compound does not necessarily mean the player understands which case attribute it counteracts.

## Suggested logical records

### Case profile

- Case identifier
- Set/array of attribute IDs
- Campaign phase
- Completion state

### Compound

- Compound identifier
- Set/array of molecule IDs
- Display name (if needed)
- Catalogue/discovery state

### Inventory entry

- Compound identifier
- Quantity or ownership count

### Research discovery

- Attribute identifier
- Corresponding molecule identifier
- Whether the relationship has been discovered

### Player progression

- Current case
- Completed cases
- Money
- Current energy
- Machine upgrade level / shared upgrade level

## Data rules

- Attribute and molecule identifiers should be stable IDs, not display names.
- Molecule collections should behave as sets: no duplicate IDs.
- Compound blueprints persist after physical compounds are consumed.
- Research discoveries persist once learned.
- Cure validation should compare normalized molecule sets, not array order.
- Avoid storing redundant per-case cure recipes. Derive the required molecule set from the case's attributes and the research mapping.
