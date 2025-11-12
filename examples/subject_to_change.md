# Measuring Organizational Transformation in Armed Groups at Scale

**Publication:** *Political Science Research and Methods (2024)*  
**Research Question:** How can we systematically measure organizational transformation in armed conflict actors when internal processes are strategically concealed and data availability is inconsistent across contexts?  

**Methods:** 
  - Measurement: structural topic modeling on UCDP event source texts
  - Inference: Cox proportional hazards models for conflict termination
  
**Scale:** 258 armed groups, 191,252 events, 1989–2020  

---
## Role as a PRISM example

**Demonstrates Complete Workflow:**

- Explicit diagnosis of the opacity problem  
- Theoretically grounded mapping of observables  
- Principled computational measurement  
- Applied inference testing predictions  
- Rigorous validation and scope conditions  
- Transparent about inferential limits  

**Achieves Scale:**  
258 groups across 30+ years — true computational social science.

**Creates Infrastructure:**  
Reusable models and pipelines for replication or extension.

**Bridges Traditions:**  
Connects qualitative theory, quantitative conflict research, and computational text analysis.

**Key Innovation:**  
Demonstrates how to infer hidden processes at scale through text-based behavioral traces.

---


## DESIGN

### Step 1: Diagnose the Problem

**Target Concept:** Organizational transformation in armed groups — the internal shifts, strategic recalibrations, and operational changes that theory predicts affect conflict dynamics.

**Why Data Is Unavailable:**

- Strategic concealment: Armed groups actively hide internal deliberations, strategic planning, and organizational restructuring.  
- Structural limitations: Even when internal documents exist, they're inaccessible to researchers.  
- Temporal constraints: Historical conflicts have sparse documentation; contemporary conflicts have uneven media access.  
- Conceptual ambiguity: "Transformation" is inherently amorphous—no consensus on consistent metrics.  

**What's Observable vs. Inaccessible:**

- **Inaccessible:** Internal negotiations, factional debates, leadership succession dynamics, resource allocation decisions, strategic planning documents  
- **Observable:** News reports of group activities, which embed both behavioral patterns and contextual descriptions  
- **Observable:** Temporal patterns in how groups are described and what actions are attributed to them  

**Key Diagnostic Questions:**

- Can we measure organizational change through behavioral manifestations rather than internal processes?  
- Is news coverage systematic enough to capture transformation at scale?  
- What threshold of change is substantively meaningful vs. noise?  

**Reframing Strategy:**  
Pivot from unobservable internal transformation to observable representational shifts in news coverage. If groups undergo genuine organizational change, this should manifest in systematic shifts in how they're described and what activities are attributed to them — a revealed preferences approach.

---

### Step 2: Map the Hidden System

**Theoretical Scaffold:** Organizational transformation in armed groups involves:

- Changes in strategic priorities (targets, tactics, territorial ambitions)  
- Operational shifts (capability evolution, tactical repertoires)  
- Factional realignments (leadership changes, internal conflicts)  
- External positioning (alliances, rhetoric, public messaging)  

**Touchpoints with the Observable World:**  

- **Activities:** What groups do (attacks, territorial control, negotiations)  
- **Context:** How groups are described (ideological framing, organizational descriptors, relationship to other actors)  
- **Temporal patterns:** Changes in activity frequency, intensity, target selection  

---

### Step 3: Theory as Structure

**Mechanism to Proxy:**  
Internal organizational transformation → Behavioral and operational shifts → Systematic changes in how activities are reported and groups are described

**Observable Implications if Transformation Occurs:**

- Temporal clustering: Coverage themes should shift coherently, not randomly fluctuate.  
- Magnitude: Genuine transformation should produce substantial representational change.  
- Persistence: Changes should persist rather than immediately revert.  
- Correlation with conflict dynamics: If transformation creates uncertainty, it should associate with conflict intractability (following Nilsson & Svensson’s theoretical logic).

**Alternative Explanations:**

- Media attention shifts unrelated to actual organizational change  
- Coverage bias toward spectacular events masks underlying continuity  
- Changes in reporter access or information sources  
- Environmental shocks (government crackdowns) that change context without organizational transformation  

**Discrimination Strategy:**  
If representational changes reflect genuine organizational transformation, they should:

- Occur at theoretically relevant moments (not randomly distributed)  
- Associate with conflict outcomes in predicted ways (uncertainty → longer conflicts)  
- Show substantive magnitude (not just statistical noise)  
- Demonstrate face validity when examined qualitatively for specific groups  

---

## TRACE AND MEASUREMENT

### Step 4: Trace Design

News coverage captures behavioral traces and second-order framing of inherently hard-to-capture markers of organizational identity. 
Year-over-year shifts in the thematic structure of news coverage should proxy underlying organizational transformation, especially when changes are rapid and substantial.

**Primary Trace Source:** UCDP Georeferenced Event Dataset (GED) v21.1 source articles  
Captures operation at scale:
- 191,252 violent events from 1989–2020  
- 352 non-state armed groups across 393 conflict dyads  
- News articles systematically selected, vetted, and deduplicated by UCDP
- 
**Design Logic:**  
Model full texts rather than event features because texts embed richer information—not just "what happened" but contextual descriptions that reveal how groups are understood and positioned.

---

### Step 5: Measurement – Bootstrapping Features

**Challenge:** Operationalize "organizational transformation"—an abstract, multidimensional concept—from heterogeneous news coverage.  

**Computational Strategy:** Structural Topic Modeling (STM)

**Why STM:**

- Unsupervised discovery (doesn't impose predetermined categories)  
- Incorporates temporal covariates (models change over time)  
- Validated for short texts on narrow topics  
- Efficient at scale

**Operationalizing “Change”:**

- **Measurement:** Magnitude of difference in topic ratio between year t and t–1.  
- **Threshold:** Change = yearly shift in topic ratios.  
- **Meaning:** Coverage shifted from predominantly one organizational frame to another.  
- **Justification:** High threshold captures rapid, substantial transformation.  

**Validation:**

- Distribution check (most group-years near zero).  
- Threshold sensitivity (|1|, |1.5|, |2|).  
- Activity correlation tests.  
- Preprocessing robustness checks.  

---

## ESTIMATION

### Step 6: Estimation and Applied Inference

**Inferential Strategy:**  
Use text-derived change measures to test theoretical predictions about organizational uncertainty and conflict dynamics.  

**Application Design:** Extension of Nilsson & Svensson (2021)  

**Original Finding:**  
Theoretical expectation that uncertainty prolongs conflict, originally operationalized by measuring whether conflicts with Islamist-motivated groups are more resistant to termination/

**Extension Logic:**  

If rapid organizational transformation creates uncertainty,  
and uncertainty prolongs conflicts,  
then groups with rapid representational changes should associate with longer conflicts.

**Triangulation:**  
Statistical finding + case-level face validity + theoretical consistency = convergent evidence that rapid organizational transformation associates with conflict intractability.

---

## EVALUATION

### Step 7: Validation, Refutation, Scope

**Plausibility Checks:**

- Temporal patterns make sense (stability common; rapid change rare but meaningful).  
- Activity correlation holds across low/high-activity groups.  
- Statistical robustness across thresholds.  
- Theoretical consistency with N&S predictions.  

**Face Validity:**  
Case studies examining whether identified change points align with known organizational events.

**Robustness Checks:**

- Selection effects (data sufficiency).  
- Media access and bias.  
- Alternative STM setups.  
- Temporal specifications.  

**Scope Conditions – What We Can Claim:**

- Rapid representational changes correlate with conflict intractability.  
- Text-based measurement identifies periods of potential transformation at scale.  
- The approach generalizes beyond conflict studies.  

**What We Cannot Claim:**

- Direct measurement of internal processes.  
- Causal effects (correlation only).  
- Perfect measurement (media noise and gaps).  
- That no change implies stability (could reflect data scarcity).  

**Sensitivity Analysis:**

- Media bias and reporting gaps.  
- Threshold dependence.  
- Topic dimensionality loss.  
- Possible confounding from external shocks.  

---

## COMPUTATIONAL METHODS FOR SUBSTANTIVE THEORY

### Step 8: Methodological and Theoretical Contribution

**Methodological Contribution:**  
Demonstrates how unsupervised text analysis can operationalize abstract organizational concepts when direct measurement is impossible.  

**Why This Matters:**

- Shows ML methods advancing substantive inference.  
- Provides principled, theoretically grounded modeling.  
- Demonstrates scalability and replicability.  
- Creates reusable infrastructure for future work.  

**Substantive Contribution:**  
Enables systematic testing of theories about organizational dynamics and conflict outcomes previously blocked by measurement limits.

**Theoretical Insight:**  
Uncertainty in conflict environments can be proxied through representational instability in news coverage. Rapid behavioral shifts manifest as descriptive instability, influencing conflict trajectories.

**Generalizability:**  
Revealed preferences approach applies to:

- Political parties (ideological shifts)  
- Firms (strategic repositioning)  
- Social movements (tactical evolution)  
- Any opaque organization observed through external activity  

**Limitations as Theoretical Probe:**

- Two-topic simplification masks multidimensionality.  
- Cannot distinguish strategic vs. tactical change.  
- Media framing may lag real transformation.  
- Representational noise is possible.  

---

**Replication Materials:** [https://doi.org/10.7910/DVN/1HNSZR](https://doi.org/10.7910/DVN/1HNSZR)  
**Full Paper:** [https://doi.org/10.1017/psrm.2024.26](https://doi.org/10.1017/psrm.2024.26)
