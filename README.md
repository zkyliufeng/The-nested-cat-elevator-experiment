# The-nested-cat-elevator-experiment
Schrödinger's Cat Nested in an Equivalence-Principle Elevator: An Analysis of the Differences among the Three Major Physical Theories Based on Observer Capability Configurations
# The Nested Cat–Elevator Experiment

Materials, program code, and anonymized test records for the paper:

> **Observer Capability Configurations and the Divergence of Physical Pictures across Three Major Theories: A Simulation Experiment with Schrödinger's Cat Nested in an Equivalence-Principle Elevator**
> [Authors]. Submitted to *Foundations of Physics* (2026).

The paper uses Generalized Agent Theory (GAT) to describe observers by five functions (control, generation, memory, output, and input). It proposes that, within a given comparison setting, an observer's capability configuration determines the structure of the effective physical picture it can construct. This repository contains the materials of the nested simulation experiment used in the paper to illustrate this proposition.

## Repository contents

| File | Description |
|---|---|
| `Schrödinger's Cat Demonstration Website Program.zip` | Source code of the Schrödinger's cat simulation program (inner layer of the apparatus). An online version runs at <https://schrodingers-cat.org>. |
| `External state of the elevator in the equivalence principle.ppt` | Elevator-environment demonstration (outer layer). It shows either a rocket accelerating through space or an elevator at rest on Earth's surface. |
| `Test Records of the Nested Cat–Elevator Experiment.zip` | Anonymized raw records of all 25 participants (30 questionnaire rounds, 150 item records). |
| `LICENSE` | Apache License 2.0. |

## Experimental apparatus

The apparatus consists of two nested rooms.

- **Large room**: represents the equivalence-principle elevator. It contains a gravity meter whose simulated reading (9.8 m/s²) is identical in both environments, so local measurement alone cannot distinguish them.
- **Small room**: inside the large room, represents the closed Schrödinger's cat box. Laptop B runs the cat simulation program.
- **Outside the large room**: Laptop A runs the elevator-environment demonstration.

| Interface | Function |
|---|---|
| Door B | Connects the large and small rooms; opening it allows direct observation of the cat |
| Camera A and screen A | Show the elevator environment inside the large room |
| Camera B and screen B | Show the cat's state without opening door B |
| Wireless mouse A | Switches the elevator environment |
| Wireless mouse B | Operates the intervention buttons of the cat program |

## Cat simulation program

The program uses a **classical Monte Carlo model** of decay timing. It does not represent quantum superposition or measurement-induced collapse; the cat has a definite state at every program time.

| Parameter | Value |
|---|---|
| Run length | 180 s (3 min), starting with the cat alive |
| Method | One independent Bernoulli trial per second |
| Per-second decay probability *p* | 0.384% (λ = 0.00384 s⁻¹) |
| Half-life | ≈ 180 s |
| Survival probability at end of run | ≈ 50% |

Each second, a random number *r* ∈ [0, 1) is drawn; if *r* < *p*, the decay event occurs, the hammer falls, and the cat dies. The program also provides two intervention buttons:

- **Scissors**: cuts the trigger so that the hammer falls, breaking the poison bottle and setting the cat's state to dead.
- **Protective Shield**: lowers a glass cover that shields the cat from the poison; if the cat is already dead, it restores the cat to the alive state. This restoration is a preset intervention rule of the simulation.

The **Start** and **Reset** buttons start and restart a run. Manual interventions and the random program run were recorded separately.

**Running the program**

- Online: open <https://schrodingers-cat.org>.
- Locally: unzip the program archive and open `index.html` in a modern web browser (Chrome, Edge, or Firefox). No installation is required.

## Observation conditions

Twenty-five participants were each tested under one of five conditions (five per condition). The PTAC index identifies the ideal observer role each condition simulates; it is not a measurement of participants' actual capabilities.

| Condition | Simulated role | PTAC index | Available channels and interfaces |
|---|---|---|---|
| R1 | α endpoint (zero capability) | #1 | Blindfold and earplugs; no channels or interfaces |
| R2 | Typical finite observer that interacts with the system (quantum) | #122 | Gravity meter; door B (answers before and after opening) |
| R3 | Observer omniscient within its domain but with no access beyond it (relativity) | #236 | Gravity meter; camera B and screen B |
| R4 | Omniscient observer that does not intervene (classical mechanics) | #237 | Gravity meter; cameras A and B, screens A and B |
| R5 | Ω endpoint (ideally infinite capability) | #243 | All channels and both mice |

## Test records

The test records contain, for each participant:

- questionnaire responses (items Q1–Q5, see Table 5 of the paper);
- elevator environment setting (selected by coin toss before each test);
- program state logs and state-check records;
- operation-confirmation records (condition R5).

Participants are identified only by anonymous codes **P0k-1 to P0k-5** for condition R*k* (*k* = 1, …, 5). R2 participants have two rounds, labeled "Before opening door B" and "After opening door B". For R1, items Q2–Q5 were not shown to participants and are marked "rule-filled"; these entries are not participant responses.

## Ethics

The study was approved by the Ethics Committee of the Institute for Digital Brain Research of CST (approval no. 2026-9-1). All participants gave written informed consent, including consent to the publication of anonymized results.

## Citation

If you use these materials, please cite the paper above. [Full citation and DOI to be added after publication.]

## License

Released under the Apache License 2.0. See `LICENSE` for details.
