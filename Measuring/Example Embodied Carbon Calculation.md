# Fundamental Calculation
The fundamental principle for calculating embodied carbon is to scale the physical quantity of structural material by the carbon factor of a given set of life cycle modules.

$Embodied \: Carbon = physical \: quantity ∗ carbon \: factor$

Physical quantities of mass or volume are typically used, in both metric or imperial units:

$EC_{A1-A3} [kgCO_2 e]=mass [kg] * CF_{A1-A3} \: [(kgCO_2 e)/kg]$
$EC_{A1-A3} [kgCO_2 e]=volume [yd^3] * CF_{A1-A3} \: [(kgCO_2 e)/yd^3]$

Carbon factors are developed by performing detailed life cycle assessments (LCAs) (see [[How to Perform an LCA]] for further details). These product-level LCAs are typically reported in [[Environmental Product Declarations]] (EPDs).

# Example
It's best to see this through an example. Consider the following quantity takeoff for a structural system for a 6-storey, 160,000sf composite steel frame with drilled pier foundations, and a reinforced concrete shear wall lateral system.

| Component      | Material             | Quantity | Units          |
| -------------- | -------------------- | -------- | -------------- |
| Foundation     | 4000 psi Concrete    | 896      | $yd^3$         |
|                | Rebar                | 145      | $short \: ton$ |
| Lateral System | 4000 psi Concrete    | 166      | $yd^3$         |
|                | Rebar                | 449      | $short \: ton$ |
| Floor          | 3000 psi LW Concrete | 1782     | $yd^3$         |
|                | Steel Deck           | 190      | $short \: ton$ |
| Beam           | Hot Rolled Steel     | 1923     | $short \: ton$ |
| Column         | Hot Rolled Steel     | 198      | $short \: ton$ |
To calculate the A1-A3, “cradle-to-gate” embodied carbon, we must identify carbon factors for each material. See [[Life cycle stages and modules]] for details about A1-A3.

Let’s just consider the rebar for a sample calculation. From the QTO, the total rebar quantity can be summed:

	Foundation rebar:      145 short tons
	Lateral system rebar:  449 short tons
	Total qty of rebar:    594 short ton

Now, the carbon factor for rebar for life cycle modules A1-A3 needs to be determined.

We use data from [[Environmental Product Declarations]]. For a "[Steel Reinforcement Bar](https://www.crsi.org/wp-content/uploads/CRSI_Industry-Wide_EPD_Sep2022.pdf)" industry average value published by the Concrete Reinforcing Steel Institute, we get:

	$CF_{A1-A3} = 854 kgCO_2 e /metric \: tonne$

But the units of our QTO is in short tons. So, a unit conversion is needed.

	$CF_{A1-A3} = 774 kgCO_2 e /short ton$

With the material quantity and the carbon factor, we can calculate the A1-A3 embodied carbon:

	$EC_{rebar,A1-A3}=quantity \: [short \: ton] * CF \: [\frac{kgCO_2 e}{short \: ton}]$
	$EC_{rebar,A1-A3}=594*774$
	$EC_{rebar,A1-A3}=459,756 kgCO_2 e$

We then repeat this for each material identified as part of the quantity take-off.

| Component      | Material             | Quantity | Units          | $CF_{A1-A3}$($kgCO_2 e/unit$) | $EC_{A1-A3}$ ($kgCO_2 e$) |
| -------------- | -------------------- | -------- | -------------- | ----------------------------- | ------------------------- |
| Foundation     | 4000 psi Concrete    | 896      | $yd^3$         | 251                           | 224,896                   |
|                | Rebar                | 145      | $short \: ton$ | 774                           | 112,230                   |
| Lateral System | 4000 psi Concrete    | 166      | $yd^3$         | 251                           | 41,666                    |
|                | Rebar                | 449      | $short \: ton$ | 774                           | 347,526                   |
| Floor          | 3000 psi LW Concrete | 1782     | $yd^3$         | 367                           | 654,994                   |
|                | Steel Deck           | 190      | $short \: ton$ | 2105                          | 399,950                   |
| Beam           | Hot Rolled Steel     | 1923     | $short \: ton$ | 1107                          | 2,128,761                 |
| Column         | Hot Rolled Steel     | 198      | $short \: ton$ | 1107                          | 219,186                   |
|                |                      |          |                | Total:                        | 4,129 tonnes              |
We have computed the total embodied carbon of the structural system from the QTO to be 4,129 tonnes of $CO_2 e$. This value can be normalized by the floor area of the building, resulting in $278 kgCO_2 e / m^2$. 

These results can be broken down by material, building system, or lifecycle stage/module to provide additional insights to ultimately make reductions. This breakdown is called a 'contribution analysis'. Below is a contribution analysis separated by material for the example.

![[Contribution Analysis.png]]
# Navigation
Return: [[Home]]
Suggested Next: [[Data Collection Strategies]]