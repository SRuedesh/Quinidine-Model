# Quinidine-Model
Whole-body parent-metabolite PBPK model of quinidine as CYP2D6 perpetrator and CYP3A4 and P-gp victim drug.

This repository contains the quinidine model originally published by Feick et al. [[1](#references)] and used in the CYP2D6 drug-drug-gene interaction network by Rüdesheim et al. [[2](#references)].

The model was developed and evaluated using published clinical plasma pharmacokinetic data after intravenous or oral quinidine administration by Ochs et al. [[3](#references), [6](#references)], Maeda et al. [[4](#references)], Andreasen et al. [[5](#references)], Strum et al. [[7](#references)], Ching et al. [[8](#references)], Laganière et al. [[9](#references)], Bleske et al. [[10](#references)], Damkier et al. [[11](#references)], Edwards et al. [[12](#references)], Hardy and Schentag [[13](#references)], Kolb et al. [[14](#references)], Darbar et al. [[15](#references)], Fremstad et al. [[16](#references)], Guentert et al. [[17](#references)], Mason et al. [[18](#references)], Bolme and Otto [[19](#references)], Frigo et al. [[20](#references)], Rao et al. [[21](#references)], Kaukonen et al. [[22](#references)] and Shin et al. [[23](#references)].

Users of the model are expected to cite these studies when using the model in scientific work, reports or derivative model development:
- [D Feick, S Rüdesheim, F Z Marok, D Selzer, H L H Loer, D Teutonico, S Frechen, M van der Lee, D J A R Moes, J J Swen, M Schwab, T Lehr. Physiologically-Based Pharmacokinetic Modeling of Quinidine to Establish a CYP3A4, P-gp and CYP2D6 Drug-Drug-Gene Interaction Network. CPT Pharmacometrics Syst Pharmacol, 2023;12:1143-1156.](https://doi.org/10.1002/psp4.12981)
- [S Rüdesheim, H L H Loer, D Feick, F Z Marok, L M Fuhr, D Selzer, D Teutonico, A R P Schneider, J Solodenko, S Frechen, M van der Lee, D J A R Moes, J J Swen, M Schwab, T Lehr. A Comprehensive CYP2D6 Drug-Drug-Gene Interaction Network for Application in Precision Dosing and Drug Development. Clin Pharmacol Ther, 2025.](https://pubmed.ncbi.nlm.nih.gov/39953671/)

This quinidine model is intended to describe quinidine and 3-hydroxyquinidine pharmacokinetics and to support CYP3A4, P-gp and CYP2D6 drug-drug-gene interaction simulations.

The presented model includes the following features:

- metabolism by CYP3A4,
- formation of 3-hydroxyquinidine,
- P-gp transport,
- CYP2D6 inhibition,
- renal filtration and secretion,
- oral absorption with Weibull dissolution.

## Repository files
This repository contains:

- a [PK-Sim snapshot (*.json) file](https://docs.open-systems-pharmacology.org/working-with-pk-sim/pk-sim-documentation/importing-exporting-project-data-models#exporting-project-to-snapshot-loading-project-from-snapshot) of the current PBPK model
- static content (e.g. text blocks, *.md files) as inputs for an evaluation plan
- an evaluation plan (evaluation_plan.json) to create an evaluation report using the snapshot and static text blocks to display the performance of the model

**The latest release of the snapshot of the model, the evaluation plan and the static content can be found in the [latest release in this repository](../../releases/latest).**

**The latest release of the PK-Sim project model file and the respective evaluation report can be found in the [latest OSP PBPK Model Library release](https://github.com/Open-Systems-Pharmacology/OSP-PBPK-Model-Library/releases/latest).**

## Code of conduct
Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution
We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License
The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References
[1] [D Feick, S Rüdesheim, F Z Marok, D Selzer, H L H Loer, D Teutonico, S Frechen, M van der Lee, D J A R Moes, J J Swen, M Schwab, T Lehr. Physiologically-Based Pharmacokinetic Modeling of Quinidine to Establish a CYP3A4, P-gp and CYP2D6 Drug-Drug-Gene Interaction Network. CPT Pharmacometrics Syst Pharmacol, 2023;12:1143-1156.](https://doi.org/10.1002/psp4.12981)

[2] [S Rüdesheim, H L H Loer, D Feick, F Z Marok, L M Fuhr, D Selzer, D Teutonico, A R P Schneider, J Solodenko, S Frechen, M van der Lee, D J A R Moes, J J Swen, M Schwab, T Lehr. A Comprehensive CYP2D6 Drug-Drug-Gene Interaction Network for Application in Precision Dosing and Drug Development. Clin Pharmacol Ther, 2025.](https://pubmed.ncbi.nlm.nih.gov/39953671/)

[3] [H R Ochs, E Grube, D J Greenblatt, E Woo, G Bodem. Intravenous quinidine: pharmacokinetic properties and effects on left ventricular performance in humans. Am Heart J, 1980;99:468-475.](https://doi.org/10.1016/0002-8703(80)90381-6)

[4] [K Maeda, J Takano, Y Ikeda, T Fujita, Y Oyama, K Nozawa, Y Kumagai, Y Sugiyama. Nonlinear pharmacokinetics of oral quinidine and verapamil in healthy subjects: a clinical microdosing study. Clin Pharmacol Ther, 2011;90:263-270.](https://doi.org/10.1038/clpt.2011.108)

[5] [A H Andreasen, K Brøsen, P Damkier. A comparative pharmacokinetic study in healthy volunteers of the effect of carbamazepine and oxcarbazepine on CYP3A4. Epilepsia, 2007;48:490-496.](https://doi.org/10.1111/j.1528-1167.2007.00924.x)

[6] [H R Ochs, D J Greenblatt, E Woo, K Franke, H J Pfeifer, T W Smith. Single and multiple dose pharmacokinetics of oral quinidine sulfate and gluconate. Am J Cardiol, 1978;41:770-777.](https://doi.org/10.1016/0002-9149(78)90830-5)

[7] [J D Strum, J L Colaizzi, J M Jaffe, P C Martineau, R I Poust. Comparative bioavailability of four commercial quinidine sulfate tablets. J Pharm Sci, 1977;66:539-542.](https://doi.org/10.1002/jps.2600660420)

[8] [M S Ching, S L Elliott, C K Stead, R T Murdoch, S Devenish-Meares, D J Morgan, R A Smallwood. Quinidine pharmacokinetics and pharmacodynamics are unaltered by omeprazole. Aliment Pharmacol Ther, 1991;5:523-531.](https://doi.org/10.1111/j.1365-2036.1991.tb00521.x)

[9] [S Laganière, R F Davies, G Carignan, et al. Pharmacokinetic and pharmacodynamic interactions between diltiazem and quinidine. Clin Pharmacol Ther, 1996;60:255-264.](https://doi.org/10.1016/S0009-9236(96)90052-1)

[10] [B E Bleske, P L Carver, T M Annesley, J R M Bleske, F Morady. Effect of ciprofloxacin on quinidine pharmacokinetic and ECG parameters. J Clin Pharmacol, 1990;30:911-915.](https://doi.org/10.1002/j.1552-4604.1990.tb03570.x)

[11] [P Damkier, L L Hansen, K Brøsen. Rifampicin treatment greatly increases apparent oral clearance of quinidine. Pharmacol Toxicol, 1999;85:257-262.](https://doi.org/10.1111/j.1600-0773.1999.tb02019.x)

[12] [D J Edwards, R Lavoie, H Beckman, R Blevins, M Rubenfire. Effect of verapamil on quinidine pharmacokinetics and metabolism. Clin Pharmacol Ther, 1987;41:68-73.](https://doi.org/10.1038/clpt.1987.11)

[13] [B G Hardy, J J Schentag. Lack of effect of cimetidine on the metabolism of quinidine: effect on renal clearance. Int J Clin Pharmacol Ther Toxicol, 1988;26:388-391.](https://pubmed.ncbi.nlm.nih.gov/3220613/)

[14] [K W Kolb, W R Garnett, R E Small, G W Vetrovec, B J Kline, T Fox. Effect of cimetidine on quinidine clearance. Ther Drug Monit, 1984;6:306-312.](https://doi.org/10.1097/00007691-198409000-00009)

[15] [D Darbar, S Dell'Orto, K Mörike, G R Wilkinson, D M Roden. Dietary salt increases first-pass elimination of oral quinidine. Clin Pharmacol Ther, 1997;61:292-300.](https://doi.org/10.1016/S0009-9236(97)90161-2)

[16] [D Fremstad, O G Nilsen, L Storstein, J Amlie, S Jacobsen. Pharmacokinetics of quinidine related to plasma protein binding in man. Eur J Clin Pharmacol, 1979;15:187-192.](https://doi.org/10.1007/BF00563104)

[17] [T W Guentert, N H Holford, P E Coates, R A Upton, S Riegelman. Quinidine pharmacokinetics in man: choice of a disposition model and absolute bioavailability studies. J Pharmacokinet Biopharm, 1979;7:315-330.](https://doi.org/10.1007/BF01062532)

[18] [W D Mason, J O Covinsky, J L Valentine, K L Kelly, O H Weddle, B L Martz. Comparative plasma concentrations of quinidine formulations. J Pharm Sci, 1976;65:1325-1329.](https://doi.org/10.1002/jps.2600650916)

[19] [P Bolme, U Otto. Dose-dependence of the pharmacokinetics of quinidine. Eur J Clin Pharmacol, 1977;12:73-76.](https://doi.org/10.1007/BF00561409)

[20] [G M Frigo, E Perucca, M Teggia-Droghi, G Gatti, A Mussini, J Salerno. Comparison of quinidine plasma concentration curves after oral formulations. Br J Clin Pharmacol, 1977;4:449-454.](https://doi.org/10.1111/j.1365-2125.1977.tb00760.x)

[21] [B R Rao, D Rambhau. Absence of a pharmacokinetic interaction between quinidine and diazepam. Drug Metabol Drug Interact, 1995;12:45-51.](https://doi.org/10.1515/dmdi.1995.12.1.45)

[22] [K M Kaukonen, K T Olkkola, P J Neuvonen. Itraconazole increases plasma concentrations of quinidine. Clin Pharmacol Ther, 1997;62:510-517.](https://doi.org/10.1016/S0009-9236(97)90046-1)

[23] [J G Shin, W K Kang, J H Shon, M Arefayene, Y R Yoon, K A Kim, D I Kim, D S Kim, K H Cho, R L Woosley, D A Flockhart. Possible interethnic differences in quinidine-induced QT prolongation between healthy Caucasian and Korean subjects. Br J Clin Pharmacol, 2007;63:206-215.](https://doi.org/10.1111/j.1365-2125.2006.02793.x)
