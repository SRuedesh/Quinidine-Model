The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](References.md)). Relevant information on anthropometric and physiological parameters in adults was gathered from the literature and incorporated into PK-Sim as default values for adult simulations ([Willmann 2007](References.md)).

The applied activity and variability of plasma proteins and active processes integrated into PK-Sim are described in the publicly available PK-Sim Ontogeny Database or otherwise referenced for the specific process.

The quinidine model was developed as a parent-metabolite PBPK model for quinidine and 3-hydroxyquinidine by [Feick 2023](References.md). Model development used intravenous and oral clinical data to inform distribution, oral absorption, P-gp transport, CYP3A4-mediated metabolism, metabolite disposition, and renal elimination.

Clinical studies used for model building were selected to cover key structural information, including intravenous dosing, nonlinear oral exposure, repeated dosing, and metabolite observations. Verification simulations used independent oral and intravenous study arms, different dose levels and formulations, salt-intake conditions, and inhibitor or inducer scenarios. This split preserves the training and test logic used for model evaluation.

The intravenous data support systemic distribution, renal elimination, and parent-metabolite disposition without the need to estimate oral absorption. Oral and repeated-dose studies then support absorption, nonlinear exposure, enterohepatic circulation, and transporter-related assumptions. The use of parent, metabolite, and unbound quinidine observations provides complementary checks on the structural model.

The model contains CYP3A4 metabolism to 3-hydroxyquinidine, P-gp transport, P-gp-mediated renal secretion, passive renal filtration, enterohepatic circulation, and CYP2D6 inhibition. Because quinidine is both a victim and a perpetrator compound, parent quinidine, 3-hydroxyquinidine, and unbound quinidine observations need to be interpreted separately where available.

The evaluated applications include intravenous infusion, oral solution, oral capsule, oral tablet, single-dose, and multiple-dose dosing. The major proteins and processes represented explicitly are CYP3A4, P-gp, CYP2D6 inhibition, plasma protein binding, passive renal filtration, renal secretion, and enterohepatic circulation. These processes make the quinidine model broader than a clearance-only substrate model.

The report therefore evaluates total quinidine, unbound quinidine, and 3-hydroxyquinidine profiles where available. Model-building profiles are used to establish the structural assumptions, while verification profiles test whether the model can reproduce independent dose, formulation, and interaction scenarios without additional fitting.

Details about input data are provided in Section 2.2. Details about the structural model and assumptions are provided in Section 2.3.
