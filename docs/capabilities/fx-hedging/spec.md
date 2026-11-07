Currency: USD/EUR (or specify applicable currency pair)
Notional Amount: 17,500,000
Settlement Date: $19,547,500 at a baseline spot rate of 1.1170 ($S_0$)
Business Consequence of an Adverse Move: If the euro depreciates prior to settlement (e.g., falling to 1.0500, reducing proceeds to $18,375,000), conversion proceeds shrink proportionally, directly eroding corporate operating margins, cash flow stability, and net export profitability.
NAMED RANGE,PLACEHOLDER VALUE,UNIT,STAGE-4 DATA SOURCE
FC_AMT,"17,500,000",EUR,Commercial Invoice / ERP
S0_in,1.1170,USD per EUR,Market Treasury Feed (Indicative)
F0_in,1.12645,USD per EUR,Theoretical Forward Curve (Indicative)
R_USD,0.04285,Annual % (ACT/360),U.S. SOFR Curve (Indicative)
R_FC,0.02590,Annual % (ACT/360),EURIBOR Curve (Indicative)
K_PUT,1.1170,USD per EUR,Execution Ticket / At-The-Money (Indicative)
K_CALL,1.1170,USD per EUR,Execution Ticket / At-The-Money (Indicative)
PREM_PUT,0.0194,USD,Derivative Pricing Desk (Indicative)
PREM_CALL,0.0150,USD,Derivative Pricing Desk (Indicative)
T_DAYS,182,Days,Contractual Due Date
