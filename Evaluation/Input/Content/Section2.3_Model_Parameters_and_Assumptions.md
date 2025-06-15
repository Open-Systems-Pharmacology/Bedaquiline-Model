### Absorption <a id="model-parameters-and-assumptions-absorption"></a>

Bedaquiline oral absorption is atypical with delay and double peaks. A Weibull function was selected in PK-Sm to describe the atypical absorption profile of bedaquiline and parameter identification was performed to fit weibull parameters (`Weibull dissolution time (50% dissolved)` and `Weibull dissolution shape`) to observed plasma concentrations.

### Distribution <a id="model-parameters-and-assumptions-distribution"></a>

Distribution is affected by lipophilicity and fraction unbound, for which different values have been reported in literature. The selected values (see [Section 2.2.1  2.2.1	In vitro / physico-chemical Data ](#methods-data)) capture best the PK of bedaquiline and M2 in plasma.

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `PK-Sim Standard` and cellular permeability calculation by `PK-Sim Standard`. 

### Metabolism and Elimination <a id="model-parameters-and-assumptions-metabolism-and-elimination"></a>

For bedaquiline, CYP-mediated metabolism was implemented as in vitro Michaelis-Menten kinetics. The main enzyme involved in the conversion is CYP3A4, but experimental data suggests involvement of CYP2C8 and CYP2C19. The CYP expression profiles are based on RNA-sequencing (RNA-seq) method obtained from the Bgee database accessible within PK-Sim ([Cordes 2023](#main-references)). For all CYP enzymes, the `Km` was taken from literature and the `Vmax` was optimized based on clinical data (see [Section 2.2.2 Clinical Data](#methods-data)). CYP2C19 was estimated to not play a role and thus removed from the final model. Additional hepatic clearance of bedaquiline was obtained from literature. For M2, total hepatic clearance was implemented by estimating `Plasma clearance` based on PK data. 

### Automated Parameter Identification <a id="model-parameters-and-assumptions-parameter-identification"></a>

This is the result of the final parameter identification.

| Model Parameter      | Optimized Value | Unit |
| -------------------- | --------------- | ---- |
|**Bedaquiline**|
| `Weibull dissolution time (50% dissolved)` | 125.21                |      |
| `Weibull dissolution shape` | 1.51                |      |
| `Vmax` (CYP3A4) | 407.858                | µmol/L/min     |
| `Vmax` (CYP2C8) | 163.73                | µmol/L/min     |
|**N-desmethyl bedaquiline (M2)**|
| `Plasma clearance` (total hepatic clearance) | 0.14                | L/h/kg     |
