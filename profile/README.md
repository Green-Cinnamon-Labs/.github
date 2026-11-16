# Green Cinnamon Labs

**An independent open-source lab for dynamic systems, industrial computing, and experimental software research.**

> **Don't avoid the mud.** Useful abstractions should survive contact with real, messy systems.

Green Cinnamon Labs is a home for projects that begin as research questions and grow through working software. Repositories live here when they are meant to become shared environments rather than remain attached to a single author: documented experiments, reusable tools, and collaborative systems developed in public.

## Why "Green Cinnamon"?

In Portuguese, *canela* means both **cinnamon** and **shin**. The name is a deliberate wordplay on *canelas-verdes*, the traditional nickname associated with people from Vila Velha, Espírito Santo, Brazil.

One widely repeated version of the local story traces the nickname to people wading ashore through the shallow water, algae, and mud around Prainha: they returned with green-stained shins. Other versions connect it to Indigenous inhabitants, fishermen and shellfish gatherers, or green garments worn by early Portuguese arrivals. The story has variants; the image remains part of Vila Velha's cultural identity.

The leg icon keeps that wordplay visible. **Don't avoid the mud** turns it into the lab's working principle: meaningful progress rarely begins on clean, prepared ground. We choose to enter difficult terrain, understand it, and build a way through it.

## What we explore

- **Dynamic systems and simulation** - deterministic runtimes, numerical integration, and composable process models.
- **Industrial and cyber-physical systems** - process simulation, OPC-UA, supervisory control, and human-machine interfaces.
- **Distributed and cloud-native control** - Kubernetes operators, declarative policies, and event-driven architectures.
- **Experimental computing** - persistent model memory, scientific notebooks, and reproducible technical research.

## Research lines

Each line has a hub, a `spec-*` repository named after a figure whose story mirrors what the line does. The hub holds what the line knows today, its book and the issues that span repositories. Lines are allowed to cross and to draw from the same sources.

| Line | Hub | What it explores | Repositories |
|---|---|---|---|
| **Pítia** | [`spec-pitia`](https://github.com/Green-Cinnamon-Labs/spec-pitia) | Quantum computing: how quantum computers work, physical implementations, error correction, the problems they are expected to solve; following arXiv | the notebooks live in the hub |
| **Mnemósine** | [`spec-mnemosine`](https://github.com/Green-Cinnamon-Labs/spec-mnemosine) | AI engineering: training and improving models, frameworks; persistent latent memory | [`lab-latent-memory`](https://github.com/Green-Cinnamon-Labs/lab-latent-memory) |
| **Hefesto** | [`spec-hefesto`](https://github.com/Green-Cinnamon-Labs/spec-hefesto) | Supervisory applications: React, Node, Python microservices, AWS | [`tep-ihm`](https://github.com/Green-Cinnamon-Labs/tep-ihm), [`tep-historian`](https://github.com/Green-Cinnamon-Labs/tep-historian) |
| **Monjolo** | [`spec-monjolo`](https://github.com/Green-Cinnamon-Labs/spec-monjolo) | Dynamic systems simulation and numerical methods; perhaps embedded systems and a small physical plant | [`monjolo`](https://github.com/Green-Cinnamon-Labs/monjolo), [`tep-plant`](https://github.com/Green-Cinnamon-Labs/tep-plant), [`tep-optimizer`](https://github.com/Green-Cinnamon-Labs/tep-optimizer) |
| **Gajeiro** | [`spec-gajeiro`](https://github.com/Green-Cinnamon-Labs/spec-gajeiro) | Industrial supervision with Kubernetes | [`plant-supervisor`](https://github.com/Green-Cinnamon-Labs/plant-supervisor), [`tep-lab`](https://github.com/Green-Cinnamon-Labs/tep-lab) |
| **Sísifo** | [`spec-sisyphus`](https://github.com/Green-Cinnamon-Labs/spec-sisyphus) (private) | Blockchain, and the algorithms behind it | `sisyphus-network-router`, `-node`, `-gateway` (private) |

### The shared plant

Hefesto, Monjolo and Gajeiro all run on the same simulated plant: the Tennessee Eastman process (Downs and Vogel, 1993), rewritten in Rust. [`spec-tennessee-eastman`](https://github.com/Green-Cinnamon-Labs/spec-tennessee-eastman) records how that system was built and is the common reference for the three lines.

All work is tracked on one board, [GCLabs](https://github.com/orgs/Green-Cinnamon-Labs/projects/12), with a *Line* field.

## How the lab is organized

- **`spec-*`** repositories are the hubs of the research lines.
- **`lab-*`** repositories contain prototypes and exploratory experiments.
- **Named projects** such as `monjolo` are reusable systems intended to stand on their own.
- **`tep-*`** repositories are components of the shared Tennessee Eastman plant and its applications.

## Collaborate

The lab is built in public and designed to make room for collaboration. If a project overlaps with your interests, start with its README and open issues, then open an issue describing the question, experiment, or contribution you would like to pursue.

Contributions should favor reproducibility, explicit assumptions, small reviewable changes, and honest reporting of limitations and negative results.

