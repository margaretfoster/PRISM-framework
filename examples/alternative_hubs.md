## Microelectronics Supply Chain Analysis (NSDPI, July 2025)

**Research Question:** Can we identify substitute suppliers for critical microelectronics components given strategic opacity in actual manufacturing relationships?

**Opacity Problem:** 
- Trade data shows flows but not actual substitutability
- Firms don't disclose supplier relationships
- Manufacturing specs not in public data

**PRISM Steps Used:**
1. **Diagnose (Step 1):** Target = actual substitutability; data limited to trade flows and product codes
2. **Map System (Step 2):** Substitutability depends on technical specs, manufacturing capability, and existing relationships
3. **Trace Design (Step 4):** Altana shipping data, HS codes, firm-level transaction patterns
4. **Measurement (Step 5):** Network analysis of trade patterns, UMAP embeddings for similarity
5. **Stopped here:** Analysis remained descriptive (lock-in patterns, network structure) rather than moving to causal inference about what enables/prevents substitution

**Extension Pathways:**
- Estimation and Evaluation: Test mechanisms for why substitution fails (technical vs. political barriers)
- Falsification: Do we see substitution in lower-stakes components?
- What would be needed: firm-level capability data, policy experiment

**Good Example For:** Trace → Measurement → Validation cycle; also good for "when to stop at description"
