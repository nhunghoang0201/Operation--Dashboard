# Operation Dashboard

## I. Introduction
### 1.1. Situation
The Manufacturing Division is responsible for executing production plans assigned by the Planning Department. Once raw materials are procured and stocked, production begins. Completed products are stored in various warehouses to support logistics and customer distribution.

### 1.2. Complication
In practice, the actual production completion time often deviates from the plan. Additionally, during inbound quality checks, defective products may be identified and rejected, affecting delivery timelines and inventory accuracy. This inconsistency in both timeliness and quality poses challenges for operational efficiency and strategic decision-making.

### 1.3. Question
How can we deliver a data-driven, interactive dashboard to help the Head of Manufacturing monitor production progress, identify bottlenecks, and make informed decisions to improve on-time delivery and product quality?

## II. Dashboard
### 2.1. Data Dictionary: https://dataedo.com/samples/html/AdventureWorks/doc/AdventureWorks_2/modules/Manufacturing_81/module.html

### 2.2. Dashboard Link:
 https://drive.google.com/drive/u/0/folders/1d7041TK4Su2GVSPPHiTRLcO4Wf_dSpul
 
## III. Analysis & Recommendation
### 3.1. Plan adherence analysis & Recommendation
#### Insight 1:
Production volume peaks in June–August and October–November which Aligh with seasonal demand Summer (outdoor activity, bicycle purchases) & Year-end holidays (Black Friday, Cyber Monday, Christmas, New Year). However, on-time delivery rate remains stable as having xtrong production management during these peak periods.
#### => Recommendation: Proactively plan for peak seasons by securing materials and production capacity early.

#### Insight 2: 
Week 2 & 3 of each month have the highest output but the lowest on-time rates: Week 2 and Week 3 is account for  78.31% and 77.54%, respectively. This can be explained as:
Week 1 is usually used for planning, demand analysis, material prep, and machine maintenance.
Week 4 is for closing activities, inventory, KPI reviews.
#### => Recommendation: Distribute production more evenly across all weeks to reduce overload and delay risks.

#### Insight 3:
Component has 82.97% of the delayed quantity and have the highest late quantity among categories despite making up only 21.44% of planned volume.
Bike has 93.29% delay rate, though only 1.97% of total volume.
=> As Component is a material of Bike. Therefore, late component could lead late Bike
#### => Recommendation: 

- Increase safety stock for Components.
- Pre-produce Components to ensure timely Bike assembly.

#### Insight 4: 
Component: 1–3 in-house steps.
Bike: 1 in-house step.
Raw Component: 97.43% have 0 internal steps => Raw Component is mainly outsourced
#### => Recommendation:

- Source more external vendors with competitive quality and price for Component & Bike.
- Prioritize outsourcing low-complexity items

#### Insight 5:
Orders with >1,000 production runs have >92% on-time rate and are mainly Raw Components 
Orders with <1,000 runs: only 6.46–57.35% on-time
=> Increase capability to produce the product when production times increase
#### => Recommendation: Encourage regular, repeat production for suitable items.

#### Insight 6:
Orders >4,000 units have nearly 100% on-time rate. These are mostly Raw Components.	
=> Large orders are often better prepared and managed
#### => Recommendation: Consider consolidating smaller orders into larger batches to improve planning and material management

### 3.2. Defect analysis & Recommendation
#### Insight 1:
Week 2 & 3 have the highest defect rates.
Correlates with production overload in mid-month.
#### => Recommendation: Intensify defect controlling & monitoring during Week 2–3.

#### Insight 2:
Raw Component has 0.26% delay rate — higher than Component (0.21%) and Bike (0.18%)
=> Outsourced vendors may have lower quality control than in-house.
#### => Recommendation: 

- Reallocate to more capable vendors.
- Evaluate vendor performance regularly.
- Strengthen output QC for outsourced production.
- Establish periodic vendor quality review criteria
