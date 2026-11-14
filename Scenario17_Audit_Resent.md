# Scenario 17 — Stage 3 Build Audit

**Scenario:** 17 — `data-center-servers`  
**Workbook:** `Scenario_17_FX_Hedging_Stage_3.xlsx`  
**Scenario-supplied fixed inputs:** EUR 17,500,000; 182 days; bank forward 1.1705 USD/EUR; EUR put premium USD 0.0194/EUR; EUR call premium USD 0.0296/EUR.

## Stage 2 market inputs now entered

- Spot (`S0_in`): **1.1170 USD/EUR**
- USD annual rate (`R_USD`): **4.285%**
- EUR annual rate (`R_FC`): **2.590%**
- Put strike (`K_PUT`): **1.1170 USD/EUR** (at spot)
- Call strike (`K_CALL`): **1.1170 USD/EUR** (at spot)
- Days (`T_DAYS`): **182**

The spot and rates were supplied in the user's Stage 2 calculation. The market-close date and source were not included; these must be copied from the student's Stage 2 record before submission.

## Parity calculation and result

Using ACT/360:

- USD accumulation factor: `1 + 0.04285 × 182/360 = 1.021663056`
- EUR accumulation factor: `1 + 0.0259 × 182/360 = 1.013093889`
- CIP-implied forward: `1.1170 × (1.0216630556 / 1.0130980556) = **1.12644805**` (approximately **1.12645**)
- Bank forward quote (`F0_in`): **1.1705**
- Money-market proceeds: **$19,712,840.83**
- Forward proceeds: **$20,483,750.00**
- Money-market less forward: **$-770,909.17**

**Parity check: FAIL — material difference.** The discrepancy is much larger than rounding. Per the assignment instructions, the bank's forward quote remains `F0_in`; do not replace it with the CIP-implied rate. Verify that the spot and both interest rates are from the same Stage 2 market-close date, that the quoted rate conventions are annual ACT/360, and that the currency/rate labels have not been reversed. If the inputs are confirmed, request a bank/instructor requote and document the response.

## Audit findings

1. **Named-range contract — confirmed.** All ten required names are defined and attached to the intended input cells on the `Inputs` tab: `FC_AMT`, `S0_in`, `F0_in`, `R_USD`, `R_FC`, `K_PUT`, `K_CALL`, `PREM_PUT`, `PREM_CALL`, and `T_DAYS`.

2. **Formula construction — confirmed.** Forward proceeds, the three explicit money-market steps, and the option formulas are formula-driven and reference the named-range inputs.

3. **Sensitivity — confirmed.** Eleven formula-driven terminal exchange-rate scenarios span 95% to 105% of `S0_in` in 1% increments. The chart compares unhedged receivable proceeds, forward proceeds, money-market proceeds, and put net proceeds. The call is shown separately as the opposite EUR-payable exposure.

4. **Parity check — failed and documented.** The user-provided market inputs imply a forward rate near 1.12645, materially below the scenario bank quote of 1.1705. The money-market hedge is approximately $770,909.17 below the forward hedge. This is an open issue, not a formula result to force to pass.

5. **Option strike assumptions — updated.** Both strikes are set equal to the user-provided spot rate of 1.1170, consistent with Scenario 17's strike-at-spot instruction.

## Before submission

- Add the Stage 2 market-close **date and source** for 1.1170, 4.285%, and 2.590%.
- Verify that all three observations use consistent date, quote convention, and rate basis.
- Ask the instructor/bank for clarification or a requote if the parity difference remains after verifying the inputs.
- Replace the author field on the Cover tab.
- Open the workbook in Excel or Google Sheets to recalculate formulas and review the Validation tab.
- Include this audit note with the Stage 3 submission.
