### 2.3.1 Absorption

The model includes intravenous infusion and oral quinidine applications. Intravenous simulations do not require an absorption process. Oral quinidine absorption is represented with a Weibull formulation and compound-specific intestinal permeability.

`Weibull time`, `Weibull shape`, and `Specific intestinal permeability` were optimized to describe the available oral formulation data. The clinical dataset includes solution, capsule, tablet, and multiple-dose scenarios, so formulation assumptions are central to the oral model evaluation.

The intravenous studies constrain systemic disposition separately from oral absorption. Oral simulations then use the same systemic disposition assumptions and add the Weibull formulation parameters. This is relevant because quinidine exposure can be affected by absorption rate, P-gp transport, metabolism, renal secretion, and enterohepatic circulation.

The same formulation concept is used across oral studies, with study-specific applications defining the administered dose and dosing schedule. The model does not use separate fitted absorption parameters for each clinical study arm.

### 2.3.2 Distribution

Quinidine plasma protein binding was represented by a fraction unbound of 21%, and 3-hydroxyquinidine was represented with a fraction unbound of 31%, as summarized in Section 2.2.1.

Partition coefficients were calculated with the Rodgers and Rowland method. Unbound quinidine profiles are included where available, which helps evaluate whether total and unbound concentrations are described consistently.

Separate compound properties are used for quinidine and 3-hydroxyquinidine. This is necessary because metabolite concentrations cannot be interpreted only as scaled parent concentrations. The availability of unbound quinidine data provides an additional check on whether the protein-binding assumption is compatible with the total-concentration profiles.

Distribution was not fitted separately by formulation, dose, or interaction scenario. The same adult physiological assumptions and compound-specific binding inputs are used across the evaluated simulations.

### 2.3.3 Metabolism and Elimination

Metabolism, transport, renal elimination, and inhibition processes are represented in the model.

* CYP3A4

Quinidine is metabolized by CYP3A4 to 3-hydroxyquinidine. CYP3A4 K<sub>m</sub> was taken from *in vitro* data corrected for microsomal binding, while CYP3A4 k<sub>cat</sub> was optimized.

CYP3A4 controls parent depletion and metabolite formation. The same enzymatic pathway therefore affects quinidine and 3-hydroxyquinidine profiles in opposite directions. Metabolite data are important for evaluating whether CYP3A4 formation is plausible and not only whether parent exposure is reproduced.

* P-gp

P-gp transport is implemented for quinidine. The model includes P-gp-mediated transport relevant for intestinal handling and renal secretion.

P-gp was included because quinidine is a known transporter substrate and transporter-mediated renal secretion is part of the model structure. This process can influence both oral absorption and renal elimination, so it is evaluated together with formulation and renal profiles rather than as an isolated parameter.

* CYP2D6 inhibition

Quinidine and 3-hydroxyquinidine are represented as CYP2D6 inhibitors. The quinidine CYP2D6 K<sub>i</sub> is summarized in Section 2.2.1.

The inhibition component supports perpetrator simulations in drug-drug interaction scenarios. It is separated from the victim model components because inhibition potency should be sourced independently from parameters that describe quinidine disposition.

* Renal and residual elimination

The model includes passive renal filtration, renal secretion through P-gp, enterohepatic circulation, and 3-hydroxyquinidine unspecific hepatic clearance.

Renal elimination combines passive filtration with active secretion. Enterohepatic circulation is included to describe observed concentration-time behavior that cannot be explained by absorption and systemic clearance alone. The metabolite unspecific hepatic clearance accounts for downstream 3-hydroxyquinidine elimination.

### 2.3.4 Automated Parameter Identification

The following parameters were optimized by fitting the model to the data:

| Model Parameter |
| --- |
| `Specific intestinal permeability` |
| `Weibull time` |
| `Weibull shape` |
| P-gp k<sub>cat</sub> |
| CYP3A4 k<sub>cat</sub> |
| 3-hydroxyquinidine unspecific CL<sub>hep</sub> |

The optimized parameters were selected to cover oral absorption, transporter transport capacity, CYP3A4 formation, and metabolite elimination. Physicochemical, plasma-binding, and CYP2D6 inhibition values were kept as sourced inputs where possible. This preserves the distinction between disposition parameters fitted to quinidine clinical data and inhibition parameters used for perpetrator predictions.
