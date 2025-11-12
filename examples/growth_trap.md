# PRISM Example: Measuring Organizational Change in Al-Qaeda in the Arabian Peninsula (AQAP)

**Research Question:**  
Do recruitment influxes change organizational priorities in clandestine groups?  
Specifically, did AQAP's behavior shift following major recruitment events in ways consistent with a theorized mechanism of organizational adaptation to the preferences of the base. 
**Methods:** `Random Forest` classification on news coverage; `Structural Topic Modeling (STM)` on AQAP documents

---

## Step 1: Design

### Diagnose the Problem

AQAP is representative of a class of geopolitically important non-state actors who operate in areas where extensive measurement of ground truth is not always available to researchers.
The hypothesized mechanism -- forced adaptation by the top of the organization to the preferences of the base-- is doubly inaccessible: it captures internal states of leaders ("forced") and clandestine organizations ("organizational adaptation") 

**Target Mechanism:**  
M1: Internal organizational priority-setting and strategic adaptation in response to membership influx
M2: Adaptation against previous goals of organizational leaders.

**Data Environment:**
- **Strategic concealment:** No membership records, internal communications, very sparse decision-making documentation  
- **Structural unavailability:** post-hoc interviews or on-the-ground reporting supports mechanism, but has limited systematic coverage  
- **Conceptual gap:** No validated measures for “organizational change” in militant groups that scale beyond single-case studies  

**Reframing Strategy:**  
Pivot from unobservable internal deliberation to observable behavioral manifestations.  
If recruitment changes organizational priorities, those shifts should leave systematic traces in external behavior.

---

### Map the Hidden System

**Organizational Theory Scaffold:** Recruitment influxes create:
- Resource allocation pressures (new members require integration)
- Factional tensions (new cohorts bring different priorities)
- Strategic recalibration (expanded capacity enables new operations)
- Tactical evolution (fresh personnel enable different attack profiles)

**Observable Touchpoints:**
- Attack patterns (behavioral repertoire)
- Messaging priorities (revealed through propaganda)
- Target selection (strategic emphasis)
- Operational tempo

**Key Insight:**  
Multiple behavioral dimensions should shift *coherently* if driven by an organizational mechanism (vs. environmental noise or random variation).

---

### Structure Using Theory

**Mechanism to Test:**  
Recruitment influx → internal priority shifts → detectable behavioral changes

**Observable Implications:**
- Temporal clustering: Changes should concentrate around known influx periods  
- Multi-dimensional coherence: Attack patterns **and** messaging should shift  
- Pattern consistency: Changes should reflect organizational adaptation logic (not just scaling up)

**Alternative Mechanisms:**
- External shocks (government crackdowns, regional instability)
- Leadership succession effects
- Resource/capability constraints relaxing

**Discrimination Strategy:**  
Triangulate across data sources — if influx drives organizational change, we should see convergent signals from independent behavioral traces.

---

## Step 2: Trace and Measurement

### Trace Capture

**Trace Source 1: News Coverage → Attack Patterns**
- Event data aggregated from media reporting  
- **Features:** attack frequency, casualties, target types, geographic distribution, tactical choices  
- **Limitation:** Media bias toward spectacular events; coverage gaps in remote areas  

**Trace Source 2: AQAP Documents → Strategic Messaging**
- **Primary texts:** propaganda videos, *Inspire* magazine, leadership statements  
- **Features:** thematic emphasis, rhetorical frames, target audience signals  
- **Limitation:** Messaging may not reflect actual priorities (deliberate misdirection)

**Design Logic:**  
If both behavioral patterns (attacks) **and** strategic communication (documents) shift coherently around influx periods, this strengthens inference about the organizational mechanism vs. measurement artifact.

---

### Bootstrap Traces to Features

**Challenge:**  
Operationalize “organizational change” from heterogeneous trace data.

#### Computational Approach 1: Random Forest on News Coverage
- Classify/predict behavioral states from event features  
- Captures non-linear relationships between attack characteristics  
- Feature importance reveals which behavioral dimensions drive classification  
- **Validation:** Can model distinguish pre/post-influx periods?

#### Computational Approach 2: Structural Topic Model on AQAP Texts
- Extract latent thematic structure from propaganda corpus  
- Track topic prevalence over time  
- Identify shifts in messaging priorities  
- Test whether thematic shifts coincide with behavioral changes  

**Why These Methods:**
- `Random Forest` handles high-dimensional, non-linear patterns without strong parametric assumptions  
- `STM` allows data-driven topic discovery with temporal/covariate structure — letting documents reveal thematic shifts  

---

### Validate Features

**Validation Strategy:**
- Known cases: Do identified change points align with documented influx events?  
- Cross-validation: Hold-out test sets for RF models  
- Qualitative triangulation: Expert case knowledge on specific periods  

---

## Step 3: Estimation

**Inferential Strategy:**  
Multi-source triangulation to support mechanistic inference without causal identification.

**What’s Observable:**
- Temporal patterns in attack behavior (`Random Forest`)
- Thematic shifts in strategic messaging (`STM`)
- Correlation between behavioral and messaging changes

**What’s Indirect:**
- Organizational priority shifts (inferred from behavioral + messaging coherence)
- Causal role of recruitment (supported by timing + pattern, not identified)

**Triangulation Logic:**  
If recruitment influx drives organizational change, we expect:
- ✅ Behavioral patterns to shift around influx timing  
- ✅ Messaging priorities to shift correspondingly  
- ✅ Changes to be coherent across dimensions (not contradictory)  
- ✅ Patterns consistent with adaptation logic (not random)  

**Critical Honesty:**  
This is *not* causal identification — cannot rule out confounding, cannot estimate treatment effects.  
But triangulated evidence provides rigorous support for theorized mechanism.

---

## Step 4: Evaluation

### Design Evaluation

#### Plausibility Checks
- Timing: Do shifts cluster around known recruitment periods?  
- Magnitude: Are changes substantively meaningful?  
- Coherence: Do RF-identified behavioral changes align with STM-identified messaging shifts?  
- Face validity: Do results match qualitative case knowledge?

---

### Scope

**Scope Conditions — What We *Can* Claim:**
- Recruitment influxes are associated with systematic behavioral and messaging changes  
- Multiple independent signals triangulate to same temporal patterns  
- Pattern consistency supports an organizational mechanism over measurement artifact  
- Method successfully operationalizes abstract organizational concepts computationally  

**What We *Cannot* Claim:**
- Causal effect size of recruitment on organizational change  
- That recruitment is sufficient or necessary for change  
- Internal mechanism details (which leaders, which debates drove adaptation)  
- Generalizability to non-violent clandestine organizations  

---

### Sensitivity

**Sensitivity Factors:**
- Results depend on media coverage quality  
- STM topic interpretation requires analyst judgment  
- Cannot fully disentangle recruitment effects from correlated environmental changes  
- Model performance bounded by trace data limitations  

---

## Computational Methods as Theoretical Probe

**Methodological Contribution:**  
Demonstrates how ML tools can operationalize abstract organizational concepts when traditional measurement is impossible.

**Why This Matters for CSS/ML Audiences:**
- Shows computational methods solving substantive social science problems  
- Illustrates principled triangulation for model validation  
- Demonstrates how domain theory guides feature engineering and interpretation  
- Provides rigorous inference despite lack of causal identification  

**Theoretical Contribution:**  
Provides systematic evidence for recruitment-driven organizational change using scalable computational approaches.

**What We Learn:**
- Theorize a mechanism in a hostile data regime with geopolitical importance
- Behavioral and messaging changes cohere temporally and substantively  
- Computational measurement enables systematic analysis of hidden processes  
- Triangulation strategy supports inference even without causal identification  

---

