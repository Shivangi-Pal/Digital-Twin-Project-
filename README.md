# Digital Twin Model: Evaluating the Sustainability of Autonomous Vehicle Adoption

This project presents a system dynamics digital twin model developed using Vensim PLE to analyze whether the increasing adoption of Autonomous Vehicles (AVs) is sustainable in terms of electricity consumption, renewable capacity, and lithium resource availability.

## Problem Statement
Autonomous Vehicles (AVs) are expected to transform transportation. However, the rapid adoption of AVs brings concerns over:

Increased electricity demand

Lithium shortages for batteries

Pressure on renewable energy infrastructure

This model addresses the question:

❓ Is the mass adoption of AVs environmentally and infrastructurally sustainable over time?

## GML Framework (Goals, Measures, Levers)

Element        	Description

Goals	          Assess long-term sustainability of AV adoption across energy and resource dimensions

Measures      	No. of AVs, Electricity Demand, Installed Renewable Capacity, Lithium Shortage Ratio

Levers        	Government Incentives, Charging Infrastructure, AV Tech Advancement Rate, Renewable Growth Rate

## Model Architecture
The model is divided into three subsystems:
Each component interacts with feedback loops and external drivers.

### 1. AV Adoption Subsystem
#### Stock: No. of AVs

#### Flows: AV adoption rate, AV retirement rate

#### Drivers:

AV attractiveness factor (affected by incentives, infrastructure, tech rate)

Market resistance

Adoption saturation

#### Key Output: AV market share over time

### 2. Electricity Demand & Renewable Supply
#### Stock: Installed renewable capacity

#### Flows:

Renewable capacity addition rate

Renewable decommission rate

#### Calculated Outputs:

Electricity demand from AVs

Total electricity demand

Renewable supply gap

#### Levers:

Effect of AVs on investment in renewables

Base renewable growth rate

### 3. Lithium Resource Subsystem
#### Computed Variables:

Annual lithium demand = AVs × lithium per battery

Shortage ratio = Demand / Supply

#### Impacts:

Lithium shortage can act as a braking feedback loop on AV production (optional modeling extension).

## Key Feedback Loops

Loop Type              	Description

Reinforcing (R1)      	AV adoption → ↑ Electricity demand → ↑ Renewable investment → ↑ Installed capacity → Supports more AVs

Balancing (B1)        	↑ AVs → ↑ Lithium demand → Supply pressure → Shortage → ↓ AV production

Balancing (B2)        	↑ AV market share → Market resistance/adoption saturation → ↓ adoption rate

## Simulation Insights (Sample Outcomes)
What level of renewable energy growth is needed to keep pace with AV electricity demand?

How does policy intervention (incentives or tech investment) affect sustainability?

What is the tipping point where lithium shortages slow down adoption?

## Tools & Techniques
Software: Vensim PLE

Modeling: Stock-flow diagrams, feedback loop analysis

Approach: System dynamics and scenario-based simulation

## How to Use
Open the .mdl file in Vensim PLE.

Modify variables like:

Government Incentive

Charging Infrastructure Sufficiency

Base Renewable Growth Rate

Run simulations to observe trends over time.

## Future Enhancements
Add economic cost models and carbon footprint analysis.

Introduce policy levers: EV subsidies, battery recycling rates.

Integrate grid reliability metrics and peak demand pressures.
