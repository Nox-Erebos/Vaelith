# Vaelith — Laboratory Machines and Research Systems

> **Document status:** Working design document  
> **Scope:** The laboratory workflow, machine responsibilities, and the removal of the upgrade system.

## Core research workflow

1. **Receive a research dossier.** The dossier introduces the next specimen by its designation and a short description.
2. **Accept the assignment.** The player chooses to begin examining the specimen.
3. **Analyze the specimen.** The Molecular Microscope reveals its attributes and the molecules required for its treatment.
4. **Prepare a solution.** The player uses the Molecular Workstation to prepare and arrange the required molecules.
5. **Test the solution.** The Bioassay Simulator evaluates the proposed sequence.
6. **Complete the assignment.** Once the correct solution is established, the player advances to the next research dossier.

## 1. Research dossier

**Purpose:** Introduce the next immune-cell specimen and allow the player to accept its research assignment.

### Displays
- Specimen designation, such as `VY-01`.
- A short specimen description.
- An **Accept Research Assignment** button.

## 2. Molecular Microscope

**Purpose:** Analyze the accepted specimen and reveal its research properties.

### Reveals
- The attributes present in the specimen, using their established IDs (for example, `F1_A`).
- The exact set of molecules required for the specimen's solution.

## 3. Molecular Workstation

**Purpose:** Allow the player to prepare and arrange molecules into a proposed solution.

The workstation is where the player applies what they have learned from the microscope and their previous experiments.

### Core responsibilities
- Present available molecules to the player.
- Allow the player to select molecules.
- Allow the player to arrange selected molecules into a sequence.
- Submit the proposed sequence to the Bioassay Simulator.

### Important rules
- Molecules are compatible with an attribute family, not permanently paired with individual attributes.
- The microscope reveals the required molecule set.
- The player must determine the correct sequence through testing.
- A proposed solution must contain the required molecules and no additional molecules.
- The sequence must match the required order.

The workstation does not provide an automatic solution or reveal the correct sequence.

## 4. Bioassay Simulator

**Purpose:** Test a proposed molecule sequence against the accepted specimen's generated solution.

### Core responsibilities
- Receive the proposed sequence from the Molecular Workstation.
- Compare it with the specimen's required molecule sequence.
- Report whether the proposed solution is correct.

### Exact-match rule

A successful solution requires:
- Every required molecule to be present.
- No unrequired molecule to be present.
- Every molecule to occupy the correct position in the sequence.

A solution with the correct molecules in the wrong order is not a successful solution.

### Feedback

The simulator must communicate the outcome clearly. The precise level of feedback—such as whether it identifies an incorrect position or only reports an unsuccessful test—remains a design decision.
