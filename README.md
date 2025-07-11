
# Energy Cost Optimization Under Renewable Constraints
This project implements a linear programming model using Python and PuLP to determine the lowest-cost electricity generation mix under renewable energy share and capacity limits. The objective is to test how much wind, coal, and gas should be used to meet demand while minimizing cost and respecting decarbonization targets.

# Background
  This project was originally developed as a conceptual preparation for a commercial decarbonization initiative within a leading energy company in Europe.
  The final implementation involved more advanced models, integration with real-time market data, and proprietary forecasting tools.
  Due to confidentiality, this public version focuses on the core optimization logic used during early-stage exploration.

# Problem Description
The system consists of two electricity demand profiles:

- renewable1: 20,000 MWh

- renewable2: 40,000 MWh

- Each profile must be met using a mix of:
   Coal , Gas ,Wind

The model aims to:

- Minimize total generation cost (in PLN)

- Enforce renewable and gas limits per profile

- Respect maximum available capacity per source
Constraints
 - Minimum wind contribution:

- renewable1: ≥ 40%

- renewable2: ≥ 60%

- Maximum gas share:

   ≤ 5% for both profiles

 System-wide limits:

- Coal ≤ 30,000 MWh

- Gas ≤ 1,000 MWh

- Wind: 2,000 MWh ≤ Wind ≤ 19,000 MWh

# Cost Assumptions (PLN/MWh)
 Energy Source	Unit Cost
 Coal	40.56
 Gas	70.90
 Wind	30.00

# Technologies Used
Python

PuLP — Linear programming

NumPy, Matplotlib

(Optional for extension: CSV import/export, real AEMO data, dashboard integration)



