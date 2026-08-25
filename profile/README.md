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

## Featured work

### [monjolo](https://github.com/Green-Cinnamon-Labs/monjolo) - deterministic process simulation

An open-source Rust runtime for continuous dynamic process simulation. It provides composable dynamic models, RK4 integration, reusable sensor and actuator blocks, supervised execution, and an optional OPC-UA adapter. Monjolo was extracted from the Tennessee Eastman work so that the simulation machinery could evolve independently and be reused in other domains.

**Status:** active development  
**Stack:** Rust · numerical methods · OPC-UA · dynamic systems

### [Tennessee Eastman CPS Lab](https://github.com/Green-Cinnamon-Labs/spec-tennessee-eastman) - industrial control research

A multi-repository cyber-physical system built around the Tennessee Eastman Process benchmark. The project combines a Rust process simulator, industrial protocol integration, a Kubernetes supervisory operator, a web HMI, and reproducible experiment records.

The [specification repository](https://github.com/Green-Cinnamon-Labs/spec-tennessee-eastman) is the entry point for architecture decisions, experiment logs, and cross-repository work. The implementation is split across [`tep-plant`](https://github.com/Green-Cinnamon-Labs/tep-plant), [`tep-operator`](https://github.com/Green-Cinnamon-Labs/tep-operator), [`tep-ihm`](https://github.com/Green-Cinnamon-Labs/tep-ihm), and [`tep-supervisor`](https://github.com/Green-Cinnamon-Labs/tep-supervisor).

**Status:** active research; component integration is in progress  
**Stack:** Rust · Go · Python · Kubernetes · OPC-UA · process control

### [Latent Memory](https://github.com/Green-Cinnamon-Labs/spec-latent-memory) - persistent memory for language models

An experimental research direction investigating whether conversational history can persist as a compact learned state instead of being fully reinjected at every step. The project treats memory as a deformation of a latent space and compares vector-field updates with simpler baselines.

The [`spec-latent-memory`](https://github.com/Green-Cinnamon-Labs/spec-latent-memory) repository defines the research question and experimental strategy; [`lab-latent-memory`](https://github.com/Green-Cinnamon-Labs/lab-latent-memory) contains the working PyTorch and Hugging Face experiments.

**Status:** early experimental research  
**Stack:** Python · PyTorch · Transformers · representation learning

### [Survey on Quantum Computing](https://github.com/Green-Cinnamon-Labs/survey-quantum-computing) - reproducible research notebook

A question-driven notebook series about translating practical problems into the mathematical language of quantum computing: states, operators, spectra, preparation, and measurement. The material is organized as a progressive research trail rather than a collection of disconnected SDK demonstrations.

**Status:** in progress; currently written in Portuguese  
**Stack:** Python · Jupyter · linear algebra · quantum computing

## How the lab is organized

Repository names communicate their role:

- **`spec-*`** repositories hold research questions, architecture decisions, experiment records, and work that spans multiple implementations.
- **`lab-*`** repositories contain prototypes, validation experiments, and exploratory implementations.
- **Named projects** such as `monjolo` are reusable systems intended to stand on their own.
- **`tep-*`** repositories are components of the Tennessee Eastman CPS Lab.
- **Forks** preserve or adapt relevant upstream work; they are not presented as original Green Cinnamon Labs projects.

Projects range from usable software to open research. Each repository should state its current status, known limitations, and next questions as plainly as possible.

## Collaborate

The lab is built in public and designed to make room for collaboration. If a project overlaps with your interests, start with its README and open issues, then open an issue describing the question, experiment, or contribution you would like to pursue.

Contributions should favor reproducibility, explicit assumptions, small reviewable changes, and honest reporting of limitations and negative results.

