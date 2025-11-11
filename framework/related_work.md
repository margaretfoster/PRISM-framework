# Relationship to Existing Frameworks and Approaches

The **PRISM framework** addresses the motivating problem class—how to do rigorous inference when the target mechanism is strategically concealed or structurally unobservable—by synthesizing tools from across methodological traditions in positivist empirical social science.

---

## Framework Comparison

| Framework                | Assumption on Missingness     | Primary Goal               | Data Requirement           | PRISM’s Role                                  |
|---------------------------|-------------------------------|-----------------------------|-----------------------------|-----------------------------------------------|
| **Causal Inference**      | Observable treatment/outcome  | Identification              | Rich, clean                 | Adds structure when observability fails       |
| **Latent Causal Structure** | Random missingness           | Recover hidden DAG          | Large *n*, full covariates  | Handles strategic/adversarial missingness     |
| **PRISM**                 | Strategic concealment         | Defensible inference        | Sparse, adversarial         | Design & triangulation framework              |

---

## Conceptual Foundations

Inspired by causal inference, machine learning, econometrics, and multi-method social science, **PRISM** draws on explicit identification strategies, sensitivity analysis, and falsification logic.  
However, mainstream causal inference assumes that treatments and outcomes are observable (albeit with measurement error).

In contrast, **PRISM** addresses cases in which the key mechanism is accessible only through indirect traces.  
The framework builds on:

- **Proxy variable methods** (Wooldridge 2010)  
- **Sensitivity analysis** (Cinelli & Hazlett 2020)

but explicitly targets **strategic concealment** rather than random measurement error.

Likewise, PRISM complements **latent causal structure analysis** (e.g., Wang & Blei 2022), which recovers hidden causal graphs that generate observed data. However, latent causal structure analysis requires rich data in which missingness is random, not strategic or adversarial.

---

## Qualitative and Mixed-Methods Foundations

Equally part of PRISM’s DNA are qualitative and mixed methods—particularly the logic of **process tracing** and **triangulation** (Bennett & Checkel 2012, 2015; Seawright 2016).  
The core of the framework rests on qualitative design insights, including triangulation and the capture of hidden mechanisms through observable implications.  

PRISM **systematizes and extends** this underlying design logic for applications requiring greater scale or generalizability across contexts.

---

## Computational and Trace-Based Inference

PRISM assumes that researchers use **computational social science (CSS)** tools to extract signal from unconventional data sources.  
Tools such as:

- Text analysis  
- Network reconstruction  
- Remote sensing  

all expand the options for the **Design -> Trace & Measurement → Inference** pipeline.

PRISM structures the prior and subsequent questions:

- How to proceed when trace data does not directly address the project of interest?  
- How to evaluate the strength of designs that incorporate CSS tools?  

The framework provides structure focused particularly on the **trace → measurement → inference** step.

---

## Connection to Intelligence Analysis

PRISM shares a problem space with **intelligence analysis**, as both address reasoning under uncertainty with partial information.  
While **structured analytic techniques** (Heuer 1999) offer valuable tools, they are **practitioner-oriented**, not designed for academic inference with explicit scope conditions and external validity.

---

## Summary

The PRISM framework bridges **domain expertise in hidden processes** with the **rigorous standards of causal inference**, making explicit the trade-offs, limitations, and available inferential strategies when **concealment is fundamental**.
