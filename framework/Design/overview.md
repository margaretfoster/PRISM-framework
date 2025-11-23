## PRISM Framework Step 1: Diagnose ## 
<!--- MJF 11/23: Building out the section in Evernote as well as here; port over. - process tracing patterns to build observable implications of hidden mechanisms - structured analytic techniques
- causal graphs and DAG logic (e.g. Pearl 2009) -->

The first step towards a triangulated measurement of fundamentally unmeasurable concepts is to be clear about the problem space: which elements of the target mechanism or process are unattainable, which may be capturable through cleverness, and where the trade-offs lie.

In designing a generalizable workflow, I use the language of directed acyclic graphs (DAGs) developed by the causal inference community. PRISM leverages the ability of DAGs to formalize and structure work partitioning observable, unobservable, and latent components of a system. DAGs are also useful for decomposing large problems into multiple biased sub-designs and mapping how and where attainable traces arise in a system.




__Diagnosis__

What is the target process or mechanism? What are the observability challenges? Is the absence due to structural holes, strategic concealment, or access limitations? Is the concept fundamentally resistant to measurement, such as a latent or abstract variable? Then identify which elements of the system are observable and which are never accessible, given the constraints. Questions to address:

Is the lack of data a structural feature or measurement error?

Is reframing possible? (Eg, perspectives on insurgent-constituency relationships studied from within a rebel group versus from among a local constituency.)

Can the design be reframed to study outputs or consequences rather than the hidden process itself?
Is there a route to variation in observability, such as a natural experiment or policy change?
What would I need to see to convince a skeptical causal inference reviewer?

__Structure Using Theory__

What does the theory predict about how touchpoints translate into observable traces?

What patterns would confirm or refute the theorized mechanism versus other alternative explanations?

__Decompose Into Attainable Sub-designs__

Use domain knowledge and theoretical expectations to formalize expectations about the unobservable process. Enumerate the actions and states that accompany the unobservable process or mechanism. 
Identify which touchpoints leave accessible traces and are most informative for the desired mechanism. Map those processes and states to touchpoints in the observable world. 

Mapping the sub-processes into a table that presents sub-designs as tuples that encode design, trace, coverage, and a qualitative assessment of expected biases in the design. 

The following table suggests identifying candidate sub-designs via: a visible mechanism, coverage of the observable mechanism slice, a qualitative description of expected bias, and a qualitative estimate of the level of uncertainty in the design. The level of uncertainty in the design is the degree to which the sub-design allows precise estimation of the intended mechanism while being theoretically distinguishable from other possible explanations. 

***Triangulation Table***:
|Sub-design | Intended Mechanism | Slice Coverage | Expected Bias | Expected Level of Design Uncertanty | Attainable Trace(s) |
|---|---|---|---|---|---|
|..|..|..|..|..|..|

<!--- MJF 11/23: fill in table with the description of what each thing can be (row 1), and an example or two (rows 2..n)-->

This table allows users to summarize and present the conceptual scaffolding that they are building around the unattainable estimand. This creates an early focus point at the outset, where the researcher/analyst and potential audiences can probe and reinforce whether and how the attainable subdesigns reasonably approach the target hidden process. This creates the blueprint to either iterate and refine the trace and mechanism coverage or moderate the possible conclusions that are attainable from the research design.
