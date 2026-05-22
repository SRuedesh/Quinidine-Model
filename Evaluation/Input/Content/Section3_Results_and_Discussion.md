The PBPK model for quinidine was developed and evaluated with clinical pharmacokinetic data after intravenous and oral administration. The evaluation covers intravenous infusion, oral solution, capsule, and tablet applications, single-dose and multiple-dose regimens, quinidine and 3-hydroxyquinidine concentration-time profiles, total and unbound quinidine observations where available, and scenarios relevant to CYP3A4, P-gp, renal transport, and CYP2D6 inhibition.

The model-building data supported systemic disposition, absorption, formulation behavior, CYP3A4-mediated 3-hydroxyquinidine formation, renal elimination, P-gp transport, and enterohepatic circulation. Building studies included intravenous and oral quinidine data from [Ochs 1980](References.md), [Maeda 2011](References.md), [Andreasen 2007](References.md), [Ochs 1978](References.md), and [Strum 1977](References.md). Verification used a broad set of independent studies with oral and intravenous dosing, multiple formulations, metabolite observations, and interaction-relevant settings as summarized in Section 2.2.2.

The model quantifies CYP3A4-mediated formation of 3-hydroxyquinidine and other metabolites, P-gp transport, passive renal filtration, active renal secretion, enterohepatic circulation, and CYP2D6 inhibition. These mechanisms are all relevant to quinidine interpretation because the compound is used both as a victim drug and as a perpetrator in DDI and DDGI networks. The metabolite model is important because 3-hydroxyquinidine contributes information on CYP3A4-mediated formation and downstream clearance.

The next sections show:

1. the final model input parameters for the building blocks: [Section 3.1](Input_table.md).
2. the overall goodness of fit: [Section 3.2](GOF_diagnostics.md).
3. simulated vs. observed concentration-time profiles for the clinical studies used for model building and for model verification: [Section 3.3](Concentration_time_profiles.md).

[Feick 2023](References.md) reported two-fold agreement for quinidine concentration, AUClast, and Cmax predictions of 94%, 100%, and 100% in the training dataset and 90%, 97%, and 91% in the test dataset. For 3-hydroxyquinidine, the corresponding training values were 79%, 100%, and 80%, and the test values were 89%, 100%, and 100%. These metrics indicate that the model described most parent and metabolite concentration-time profiles and exposure metrics within conventional two-fold criteria.

In this evaluation, the merged GOF diagnostic over the included concentration observations gives GMFE values of 1.43 for quinidine, 1.45 for 3-hydroxyquinidine, and 1.43 for all observations. The similarity between parent and metabolite GMFE values supports the parent-metabolite structure, while the size and heterogeneity of the dataset require interpretation by dosing route, formulation, and analyte.

The concentration-time profiles should be reviewed separately for intravenous, immediate-release oral, sustained-release oral, and interaction-relevant studies. Intravenous studies test distribution and systemic clearance. Oral studies additionally test P-gp-mediated intestinal handling, dissolution assumptions, and enterohepatic circulation. Studies with metabolite observations test CYP3A4 formation and 3-hydroxyquinidine elimination. Unbound quinidine data provide a useful check on the protein-binding-dependent interpretation of total concentrations.

[Rüdesheim 2025](References.md) used quinidine in a larger CYP2D6 DDGI network. In that network, quinidine acts as a CYP2D6 and P-gp perpetrator and as a CYP3A4/P-gp victim. The current compound-level evaluation therefore supports, but does not by itself prove, DDGI network performance because network predictions also depend on victim-drug models and perpetrator interaction parameters.

The model is adequate for adult quinidine and 3-hydroxyquinidine simulations within the represented intravenous and oral dose range, formulations, and analytes. Remaining interpretation should be cautious for unrepresented dose regimens, populations, and DDGI network scenarios that depend on additional victim or perpetrator models.
