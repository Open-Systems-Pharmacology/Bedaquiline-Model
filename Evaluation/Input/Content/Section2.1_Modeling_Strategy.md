The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](#main-references)) Regarding the relevant anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in adults was gathered from the literature and has been previously published ([PK-Sim Ontogeny Database Version 7.3](#main-references)). The information was incorporated into PK-Sim® and was used as default values for the simulations in adults.

The  applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available PK-Sim® Ontogeny Database Version 7.3 ([Schlender 2016](#main-references)) or otherwise referenced for the specific process.


First, a PBPK model was built using patients PK data for bedaquiline and M2 after oral applications of 400 mg bedaquiline on day 1, 300 mg on day 2, and 200 mg on day 3 to 14 to find an appropriate structure to describe the pharmacokinetics in plasma. The  PBPK model was developed using a typical Black American individual, with an age of 30 year(s), weight of 60 kg and height of 170 cm. The relative tissue specific expressions of enzymes predominantly being involved in the metabolism of bedaquiline (CYP3A4 and CYP2C8) were considered.

Unknown parameters (see below) were identified using the Parameter Identification module provided in PK-Sim®. Structural model selection was mainly guided by visual inspection of the resulting description of data and biological plausibility.

Once the appropriate structural model was identified, additional parameters for tablet formulations were identified assuming a Weibull function. 

The model was then verified by simulating PK data for different dosing groups:

- 200-100 mg QD
- 400-300-200 mg QD
- 500-400-300 mg QD
- 700-500-400 mg QD
- 400 mg QD, followed by 200 mg thrice weekly


Details about input data (physicochemical, *in vitro* and clinical) can be found in  [Section 2.2](#methods-data).

Details about the structural model and its parameters can be found in  [Section 2.3](#model-parameters-and-assumptions).

