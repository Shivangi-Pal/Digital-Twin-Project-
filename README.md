#  Digital Twin Model: Evaluating the Sustainability of Autonomous Vehicle Adoption

This project presents a **system dynamics digital twin model** developed using **Vensim PLE** to analyze whether the increasing adoption of **Autonomous Vehicles (AVs)** is sustainable in terms of electricity consumption, renewable energy capacity, and lithium resource availability.

---

## 🎯 Problem Statement

Autonomous Vehicles (AVs) are poised to revolutionize transportation. However, their rapid adoption raises sustainability concerns:
-  Surging electricity demand
-  Lithium shortages for batteries
-  Increased pressure on renewable infrastructure

> **Key Question**: *Is the mass adoption of AVs environmentally and infrastructurally sustainable over time?*

---

##  GML Framework (Goals, Measures, Levers)

| Element      | Description                                                                 |
|--------------|-----------------------------------------------------------------------------|
| **Goals**    | Assess long-term sustainability of AV adoption across energy and resources |
| **Measures** | No. of AVs, Electricity Demand, Installed Renewable Capacity, Shortage Ratio |
| **Levers**   | Government Incentives, Charging Infrastructure, AV Tech Rate, Renewable Growth Rate |

---

##  Model Subsystems

### 1.  AV Adoption Subsystem

| Component            | Role                                                              |
|----------------------|-------------------------------------------------------------------|
| **No. of AVs**         | Stock representing total AVs in use                               |
| **AV adoption rate**   | Inflow driven by incentives, infrastructure, market share         |
| **AV retirement rate** | Outflow based on average AV lifespan                              |
| **Adoption saturation**| Caps growth due to resistance and market saturation               |



### 2.  Electricity Demand & Renewable Capacity

| Component                         | Role                                                       |
|----------------------------------|-------------------------------------------------------------|
| **Electricity demand from AVs**    | Product of AV count and average energy usage               |
| **Total electricity demand**       | Sum of AV and base electricity needs                       |
| **Installed renewable capacity**   | Stock showing renewable infrastructure                     |
| **Addition & decommission rates**  | Inflows/outflows based on investment and plant lifespan    |
| **Renewable supply gap**           | Gap between electricity demand and renewable capacity      |



### 3.  Lithium Resource Dynamics

| Component               | Role                                                          |
|-------------------------|---------------------------------------------------------------|
| **Annual lithium demand** | Driven by number of AVs × lithium per battery                 |
| **Global lithium supply** | Input to simulate market limitation                           |
| **Shortage ratio**        | Demand-to-supply ratio affecting future AV adoption           |



##  Feedback Loops

| Loop Type       | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Reinforcing (R1)** | More AVs → More electricity demand → More renewable investment → More capacity → Enables more AVs |
| **Balancing (B1)**   | More AVs → Higher lithium demand → Shortage → Limits future adoption     |
| **Balancing (B2)**   | Higher AV share → Market saturation/resistance → Slows new adoption     |

---

##  Simulation Insights

The model lets you explore scenarios such as:
- How much **renewable energy growth** is needed to meet future electricity demand?
- Can **policy incentives** speed up sustainable AV adoption?
- At what point does **lithium shortage** impact the AV rollout?

---

##  Tools Used

| Tool        | Purpose                             |
|-------------|-------------------------------------|
| Vensim PLE  | System dynamics modeling and simulation |
| Stock & Flow Diagrams | Modeling feedback and delay structures |
| Scenario Analysis | Exploring adoption, shortage, and supply dynamics |

---

##  How to Use

1. Open the `.mdl` file using **Vensim PLE**.
2. Modify levers such as:
   - Government Incentive
   - Charging Infrastructure
   - Base Renewable Growth Rate
3. Run simulations and analyze outputs such as:
   - Number of AVs
   - Electricity Demand
   - Renewable Capacity
   - Lithium Shortage Ratio

---

##  Future Extensions

| Feature                  | Purpose                                                              |
|--------------------------|----------------------------------------------------------------------|
| Battery recycling logic  | Model resource recovery from retired AVs                             |
| Economic modeling        | Track carbon costs, policy costs, and electricity pricing            |
| Grid capacity stress     | Evaluate impact on peak demand and blackout probabilities            |
| Real-time dashboard      | Build Power BI dashboard to visualize simulation outcomes            |


