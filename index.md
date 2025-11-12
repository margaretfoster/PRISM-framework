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

Partial-Observability Inference & Structured Measurement (**PRISM**) is a conceptual framework for reasoning when the structure of the world is only *partially observable*—for example, when actors, institutions, or technical systems deliberately conceal evidence of the mechanisms or processes we wish to understand.  

PRISM originated in computational social science work on clandestine organizational structures and expands to other “hostile data environments.” It unites three traditions:

- **Research design flow** from qualitative social science  
- **Causal-inference logic** from econometrics and statistics  
- **Measurement and representation learning** from computational social science and applied machine learning  

PRISM’s goal is to help researchers design *defensible* estimation and inference strategies in hard-to-measure domains.

The core is a **Design → Trace & Measurement → Estimation & Inference → Evaluation** workflow.  
This flow anchors inference within empirical social-science and ML architectures while acknowledging that work in opaque systems often requires *bespoke, indirect features* and *theory-centered judgment.*

## Core Process Flow

The schematic below outlines the PRISM design sequence.

<div align="left">
  <img src="assets/img/index_flow.svg" alt="PRISM Framework Flow" width="95%">
</div>

Formally, PRISM models inference as:

$T \rightarrow \hat{Z} \rightarrow Y$

where **T** are observed traces, **Ẑ** represents latent or hidden mechanisms, and **Y** is the outcome of interest.  
The framework provides a structured pathway for converting partial and strategically obscured traces (**T**) into defensible inference about hidden mechanisms (**Ẑ**) and their consequences (**Y**).

---

## Explore the Framework

- [**Design**](framework/Design/overview.md)  
- [**Trace & Measurement**](Measurement-Trace/overview.md)  
- [**Estimation & Inference**](Estimation/overview.md)  
- [**Evaluation**](Evaluation/overview.md)  

### Wider Context
- [Scope Conditions](framework/scope_conditions.md)  
- [Intellectual Lineage and Related Work](framework/related_work.md)

---

## Why PRISM?

- Provides a structured design pattern for inference under opaque conditions, such as where data are absent or adversarial  
- Bridges social-science theory, qualitative designs, and machine-learning formalism, enabling theory-driven yet scalable workflows  
- Suggests pathways to generate testable hypotheses and quantitative metrics in opaque domains  

## When to use PRISM:
PRISM is most valuable for research questions that involve strategic concealment or structural unavailability when the phenomenon doesn't leave direct traces, and when one wants to:

- Test theoretical mechanisms rather than just document patterns
- Make systematic claims when key mechanisms are hidden or when observability varies by actors or across time
- Use causal inference tools without the generous data environment assumed by standard identification strategies
- Defend a research design to audiences expecting rigorous identification strategies

## Who is PRISM for?

The PRISM framework provides a design approach for researchers working on strategically concealed or structurally unobservable processes. It's designed to help organize research design decisions and connect work to established traditions in causal inference and qualitative methods. 

Example users include:
- Researchers studying militant operations, sanctions evasion, informal economies, or other domains with strategic concealment
- Teams designing projects where standard data availability assumptions don't hold
- Analysts working on opaque domains, such as supply chain vulnerabilities and regulatory evasion.

PRISM is most valuable:

- At the early stages of research design, when thinking systematically about what is and is not observable
- For positioning research on opaque systems relative to the expectations in causal inference and qualitative communities
  
Primary audiences:

- Security and conflict researchers studying militant group operations, clandestine state programs, or terrorism
- Supply chain and economic analysts investigating sanctions evasion, informal economies, or strategic vulnerabilities in critical materials
- Computational social scientists bridging causal inference standards and measurement techniques available for hard-to-capture domains
- Analysts working in domains where ground truth is systematically hidden

---

## Resources

- [**Whitepaper (PDF)**]() — *Conceptual and technical foundations: coming soon*  
- [**Examples**](examples/) — *Case studies and examples: coming soon*

---

## Status

Version 1.0 (November 2025): Core framework with 4-step workflow, diagnostic questions, and connections to established methodological traditions.

This version provides the conceptual structure and planning guidance. Worked examples, operational tools, and domain-specific guidance will be added in future iterations based on applications and user feedback.
Contact: [m.jenkins.foster@gmail.com]

## Citation

If you use or adapt this framework, please cite:

> **Foster, Margaret. J. (2025).** *Inference Under Opacity: The PRISM Framework v1.0.*  
> [https://margaretfoster.github.io/PRISM-framework](https://margaretfoster.github.io/PRISM-framework)
---

<!-- MathJax for LaTeX rendering -->
<script>
  window.MathJax = {
    tex: {inlineMath: [['$', '$'], ['\\(', '\\)']]},
    svg: {fontCache: 'global'}
  };
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js" async></script>


© 2025 Margaret J. Foster · Released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) · View on [GitHub](https://github.com/margaretfoster/PRISM-framework)
