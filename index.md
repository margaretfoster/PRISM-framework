---
title: "PRISM Framework v1.0"
description: "Inference under partial observability and strategic opacity"
layout: home
nav_order: 1
---

# PRISM v1.0  
*A framework for inference under partial observability and adversarial data-generation processes.*

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
![Version](https://img.shields.io/badge/version-1.0--beta-blue)
![Status](https://img.shields.io/badge/status-in%20development-orange)

---

## Overview

**PRISM** (Partial-Observation Inference & Structured Measurement) is a methodological framework for reasoning when the structure of the world is only *partially observable*—for example, when actors, institutions, or technical systems deliberately conceal evidence of the mechanisms or processes we wish to understand.  

The framework originated in computational-social-science work on clandestine organizational structures and expands to other “hostile data environments.” It unites three traditions:

- **Research design flow** from qualitative social science  
- **Causal-inference logic** from econometrics and statistics  
- **Measurement and representation learning** from computational social science and applied machine learning  

PRISM’s goal is to help researchers design *defensible* estimation and inference strategies in hard-to-measure domains.

At its core lies a **Design → Trace & Measurement → Estimation & Inference → Evaluation** workflow.  
This structure anchors inference within empirical social-science and ML architectures while acknowledging that work in opaque systems often requires *bespoke, indirect features* and *structured human judgment.*

---

## Core Process Flow

The schematic below outlines the PRISM design sequence.

<div align="left">
  <img src="assets/img/index_flow.svg" alt="PRISM Framework Flow" width="95%">
</div>

Formally, PRISM models inference as:

\[
T \rightarrow \hat{Z} \rightarrow Y
\]

where **T** are observed traces, **Ẑ** represents latent or hidden mechanisms, and **Y** is the outcome of interest.  
The framework provides a structured pathway for converting partial and strategically obscured traces (**T**) into defensible inference about hidden mechanisms (**Ẑ**) and their consequences (**Y**).

---

## Explore the Framework

- [**Design**](framework/Design/overview.md)  
- [**Trace & Measurement**](Measurement-Trace/overview.md)  
- [**Estimation & Inference**](Estimation/overview.md)  
- [**Evaluation**](Evaluation/overview.md)  

### Contextual Material
- [Scope Conditions](framework/scope_conditions.md)  
- [Intellectual Lineage and Related Work](framework/related_work.md)

---

## Why PRISM?

- Provides a **structured design pattern** for inference in *negative spaces* where data are absent or adversarial  
- Bridges **social-science theory**, **qualitative designs**, and **machine-learning formalism**, enabling theory-driven yet scalable workflows  
- Suggests **pathways to generate testable hypotheses** and quantitative metrics in opaque domains  
- Designed to **grow through engagement**—extendable via open notebooks, modular code, and applied examples  

### Use PRISM when:
- Key mechanisms are hidden by design  
- Observability varies across actors or time  
- Standard identification strategies fail or data are adversarially distorted  

---

## Resources

- [**Whitepaper (PDF)**]() — *Coming soon: conceptual and technical foundations*  
- [**Examples**](examples/) — *Coming soon: applied notebooks and case studies*

---

## Citation

If you use or adapt this framework, please cite:

> **Foster, M. J. (2025).** *Inference Under Opacity: The PRISM Framework v1.0.*  
> [https://margaretfoster.github.io/PRISM-framework](https://margaretfoster.github.io/PRISM-framework)

---

## Contact

For collaboration or feedback:  
[m.jenkins.foster@gmail.com](mailto:m.jenkins.foster@gmail.com)

---

© 2025 Margaret J. Foster · Released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) · View on [GitHub](https://github.com/margaretfoster/PRISM-framework)
