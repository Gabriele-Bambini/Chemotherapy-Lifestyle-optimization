# Chemotherapy–Lifestyle Optimization

**Precision exercise-oncology: a systems framework for timing physical activity around chemotherapy.**

Exercise and chemotherapy act on overlapping molecular pathways. This project aims to model
that crosstalk for 20+ chemotherapy agents and to use the model to time movement, rest and
recovery so that treatment toxicity (cardiac, neurological) is reduced and quality of life
is protected.

> **Status: concept stage.** This repository currently holds the project statement only.
> No code, data or results exist yet. Sections marked *(planned)* describe intent, not
> delivered work.

## Research question

Can a mechanistic model that couples **drug pharmacokinetics / pharmacodynamics (PK/PD)**
with **physiological signals** (heart rate, activity, sleep, recovery) identify exercise
timing windows that lower chemotherapy-related cardiotoxicity and neurotoxicity without
compromising treatment efficacy?

## Approach *(planned)*

| Layer | Goal |
|---|---|
| **1. Evidence map** | Curate, per chemotherapy agent, the molecular targets and the exercise-responsive pathways they intersect (e.g. oxidative stress, inflammation, mitochondrial function). |
| **2. PK/PD core** | Compartmental PK/PD models for each agent, with literature-derived parameters and explicit uncertainty. |
| **3. Physiology coupling** | Link wearable-derived signals to modifiers of drug clearance, exposure and organ stress. |
| **4. Timing optimizer** | Search exercise schedules that minimise predicted toxicity subject to safety constraints. |
| **5. Validation** | Compare model predictions against published trials and, where ethically and legally possible, observational data. |

## Scope and safety

This is a research framework, **not medical advice** and not a clinical decision tool.
Nothing here should be used to alter a patient's treatment or activity plan without
oncology-team supervision.

## Repository layout *(planned)*

```
docs/        evidence maps, model specifications, protocol
src/         PK/PD models and optimizer
data/        small curated parameter tables (no patient data)
notebooks/   exploratory analyses
tests/       model and unit tests
```

## Roadmap

- [ ] Define the agent list and inclusion criteria
- [ ] Systematic evidence map of exercise–chemotherapy pathway overlap
- [ ] Reference PK/PD implementation for a first pilot agent
- [ ] Toxicity endpoints and objective function
- [ ] Pre-registered validation plan

## Author

Gabriele Bambini
