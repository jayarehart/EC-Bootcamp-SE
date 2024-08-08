Life cycle assessment (LCA) is a method of environmental accounting. LCAs track all outputs to nature, in addition to all inputs from nature, while considering all of the processes that take place during the lifecycle of the system or product.

The clearly defined framework for performing LCAs is governed by the standards [ISO 14040:2006](https://www.iso.org/standard/37456.html) and [ISO 14044:2006](https://www.iso.org/standard/38498.html).  [Wikipedia](https://en.wikipedia.org/wiki/Life-cycle_assessment) provides an in-depth summary of these standards.

When measuring the embodied carbon of a structural system, we are typically performing an "abridged" version of an LCA. But, it is still important to understand the fundamental process of conducting an LCA.

This figure, adapted from the ISO 14040 standard, summarizes each of the phases of performing an LCA. An LCA begins with the definition of a goal and scope, and an interpretation of if the scope matches the goal. If the scope supports the goal, then the inventory analysis is performed and interpreted to ensure that sufficient data is available to support the previously identified goal. From here, an impact assessment is performed, with the results interpreted to draw conclusions and make recommendations.

![[ISO_LCA_Framwork.png]]
# Defining a Goal
The goal definition is arguably to most critical part of any LCA as it sets the stage for why the assessment is being performed. A well-defined goal includes the following components:

1. What is being considered
2. The reason for performing the assessment
3. The intended audience
4. How the results of the assessment should be used

We might be wanting to perform an LCA in order to identify systems that contribute the most to the embodied carbon. Or, we might want to compare the performance of structural systems on the basis of embodied carbon. Another reason might be to just record and report the total emissions of an as-constructed building.

Each of these reasons are completely valid for wanting to perform an LCA. But, the methods that we choose to collect data will vary based upon the stated goal. These methods are defined when choosing a scope.
# Choosing a Scope
One the goal of an LCA has been clearly defined, a scope is then chosen to support the goal. The scope includes both the physical scope of what is being considered (e.g., one CMU block, or a gravity structural system) in addition to the parts of the life cycle (modules/stages).

# Inventory Analysis 
In the inventory analysis of the system, the quantity of all emissions to air, land, or water for all products or processes within the system boundary are identified.

For buildings, this consists of determining a bill of materials and identification of construction processes and matching this information to data about their emissions. 

# Impact Assessment 
The impact assessment translates the emissions inventory, which is in mass of emissions to air, land, or water (i.e., kgCO2, kgCH4, etc.), to an environmental impact (e.g., global warming) through a characterization factor. 

The [TRACI v2.2](https://www.epa.gov/chemical-research/tool-reduction-and-assessment-chemicals-and-other-environmental-impacts-traci) (Tool for Reduction and Assessment of Chemicals and Other Environmental Impacts) method, developed by the EPA, provides characterization factors for many different midpoint indicators. For climate change impacts, it provides characterization factors for greenhouse gasses that align with the IPCC:

$1 kgCO_2 = 1 kgCO_2 e$
$1 kgCH_4 = 25 kgCO_2 e$
$1 kgN_2O = 298 kgCO_2 e$
$1 R410a = 3500 kgCO_2 e$

It's important to note that different GHGs have different impacts on the climate. These are called “Global Warming Potentials” or characterization factors. For further discussion of what global warming potentials are and how they're used, see [this article by the EPA](https://www.epa.gov/ghgemissions/understanding-global-warming-potentials).

After performing an impact assessment, a final interpretation is performed to understand how the results of the LCA matched the intended goal and scope and if any other revisions to the methodology is needed.

# Example LCA Calculation
The following outlines a fundamental LCA calculation, stepping through each phase of the formal LCA framework. Typically, a structural engineer is not performing these calculations, but rather using the results of these LCA calculations from environmental product declarations (EPDs)

**Step 1. Define the Goal & Scope**
*This assessment is a study of a generic product from cradle-to-gate.*

**Step 2. Inventory Analysis**
*Perform a quantity take-off of all products and processes. Use a life cycle inventory (LCI) to determine the GHG emissions to the atmosphere:*

*Result: $70 kg CO_2$, $0.2 kg CH_4$, 0.4 $kg N_2 O$

**Step 3. Impact Assessment**
*Use TRACIv2.2 characterization factors to convert the emissions inventory to environmental impacts, specifically global warming impacts.*

$GWI=[70 kgCO_2∗1 \frac{kgCO_2 e}{kgCO_2}]+[ 0.2 kgCH_4∗25  \frac{kgCO_2 e}{kgCH_4 }]+ [0.4 kgN_2 O∗298 \frac{kgCO_2 e} {kgN_2 O}]$
$GWI=[70 kgCO_2 e]+[5 kgCO_2 e]+[119.2 kgCO_2 e]$
$GWI=194.2 kgCO_2 e$

**Step 4. Interpretation**
*At each step of the way, (1) identify issues, (2) evaluate data, (3) develop conclusions.*

# Further Readings
  
Life Cycle Assessment of Buildings (LCA): A Practice Guide. Carbon Leadership Forum (2019). v1.1. https://carbonleadershipforum.org/lca-practice-guide/

Simonen, K. (2014) Life Cycle Assessment, London, UK: Routledge. https://www.routledge.com/Life-Cycle-Assessment/Simonen/p/book/9780415702423

# Navigation
Return: [[Home]]
Suggested Next: [[Midpoint Indicators to Measure Endpoint Impacts]]