# Business Forecast Model – DQM Review Report

Nov 4, 2026 · @Ariel Gimenez

## 1. Executive Summary

### 1.1 Purpose of the Review

This report sets out the first review by Model Risk Management of the Business Forecast Model, an Excel-based tool used to produce five-year forecasts for Handelsbanken Wealth & Asset Management (HWAM). \[To be completed.\]

### 1.2 Overall Conclusion

&#91;To be completed once Sections 5 to 8 are finalised.\]

### 1.3 DQM Risk Rating

&#91;Insert rating, consistent with Section 8.\]

### 1.4 Summary of Key Findings

&#91;Insert summary of findings from Section 7.2.\]

## 2. Scope and Approach

### 2.1 Scope of Review

This is the first review of the Business Forecast Model. The review covers both versions of the tool (base case and upside forecast), which share the same structure and calculation logic. \[Confirm scope, e.g. the classification, specification, implementation and governance of the tool.\]

### 2.2 Out of Scope

&#91;To be completed, e.g. the appropriateness of individual management assumptions, or downstream processes such as ICARA and Value in Use.\]

### 2.3 Review Approach and Evidence Considered

No formal documentation was available for the DQM. The review was therefore based on the following evidence:

- Discussions with the DQM owner.
- The identification form completed by the owner.
- A review of the Excel file, covering all tabs except the stress scenario tabs, which are assessed separately.

&#91;Add any testing performed, e.g. recalculation or reasonableness checks.\]

## 3. DQM Overview, Use and Intended Purpose

### 3.1 DQM Description

The Business Forecast Model is an Excel-based tool that produces five-year forecasts of the profit and loss (P&L) of Handelsbanken Wealth & Asset Management (HWAM), together with other business forecasts. The tool is maintained in two versions that share the same structure and calculation logic and differ only in their underlying assumptions:

- **Base case forecast**, which represents the expected business outlook.
- **Upside forecast**, which aligns with the Bank's growth ambition.

The understanding set out in this report is based on discussions with the DQM owner, the identification form completed by the owner, and a review of the Excel file. No formal documentation was available for the DQM; this is addressed in Section 7.

**Workbook structure.** The Excel file is organised into the tabs below. The annual forecast covers 2026 to 2031, and the current year is also phased monthly. \[Confirm where the upside forecast is held, as it does not appear as a separate tab.\]

| Group | Tab | Purpose |
| --- | --- | --- |
| Inputs and assumptions | AUM (hidden) | Hard-coded AUM values as at September 2025, used as the forecast starting point. |
| Inputs and assumptions | Assumptions | Narrative notes on the main assumptions. Not linked to the calculation tabs. |
| Annual forecast | HWAM Base Case ICARA Scenarios | Annual operating P&L forecast for 2026 to 2031, covering AUM, yields, customers, income, costs and operating profit. |
| Annual forecast | HWAM Base Case | Appears to replicate HWAM Base Case ICARA Scenarios. Source of the forecast values in the "Summary" tab. |
| Annual forecast | Base ICARA | Annual customer acquisition and attrition forecast: customer numbers, average AUM per client, and inflows and outflows. |
| Annual forecast | Base Case | Appears to replicate Base ICARA. |
| Current year | Monthly Phased | Annual 2026 base case divided equally across the 12 months. |
| Current year | Monthly | Appears to replicate Monthly Phased. |
| Current year | 2026 P&L Revised | Monthly 2026 operating P&L, with actuals to June and forecast values from July. |
| Current year | Monthly Phased ICARA | Monthly 2026 operating P&L, cash, wind-down and capital metrics used for ICARA. |
| Outputs | Summary | Annual summary of the base case forecast, linked to the "HWAM Base Case" tab. |
| Outputs | Summary revised | As "Summary", but with 2026 linked to the "2026 P&L Revised" tab, so it reflects actuals to date. Values for 2027 onwards are the same as in "Summary". |
| Stress scenarios | ICARA S1, ICARA S2, S1 Summary, S2 Summary | Stressed versions of the ICARA scenario and their summaries. Assessed separately. |

### 3.2 Business Use and Intended Purpose

The DQM supports financial planning for HWAM. The owner has confirmed that its two versions serve distinct purposes:

- The base case forecast is used for ICARA capital and liquidity planning, and for the annual Value in Use exercise undertaken by Handelsbanken plc (PLC).
- The upside forecast is used as a benchmark against which HWAM's actual performance is assessed.

The DQM is run quarterly. \[Add examples of the other business forecasts produced, if they have separate uses.\]

#### 3.2.1 ICARA

The Internal Capital Adequacy and Risk Assessment (ICARA) is the process under the FCA's Investment Firms Prudential Regime (IFPR), set out in MIFIDPRU 7, through which an investment firm assesses whether it holds adequate own funds and liquid assets for the harms its business could cause, and plans for an orderly wind-down if needed. It is understood that HWAM, as an FCA-authorised investment firm, is subject to this requirement. \[Confirm with the owner.\]

The base case forecast supports the ICARA by projecting the HWAM P&L and its effect on capital and liquidity. The "Monthly Phased ICARA" tab rolls forward the cash balance and equity for the current year, compares own funds and liquidity against minimum requirements, and calculates wind-down amounts at 110%, 125% and 150% of a hard-coded value, assumed to be the estimated cost of an orderly wind-down. The "ICARA S1" and "ICARA S2" tabs apply stresses to the base case and are assessed separately.

**Validation observation.** The use of the DQM in the ICARA has not been clarified by the owner. In particular, MRM has not been able to confirm which outputs are reported in the ICARA, which tab they are taken from, what the hard-coded wind-down value represents and where it comes from, what the minimum requirements and BRT figures refer to, and how outputs are reviewed and approved before use.

#### 3.2.2 Value in Use

Value in Use is an accounting measure under IAS 36 *Impairment of Assets*. It is the present value of the future cash flows expected from an asset or a cash-generating unit (CGU). Each year, goodwill and certain intangible assets must be tested for impairment by comparing their carrying amount with their recoverable amount, which is the higher of Value in Use and fair value less costs of disposal. Any shortfall is recognised as an impairment loss. Under IAS 36, cash flow projections are normally based on the most recent management-approved budgets or forecasts, covering a maximum of five years, and are then extrapolated using a long-term growth rate and discounted.

The owner has confirmed that the base case forecast is used in the annual Value in Use exercise undertaken by PLC. It is assumed that the five-year base case provides the cash flow projections for HWAM as a CGU within PLC, possibly to support goodwill arising from the original acquisition of the business or PLC's investment in HWAM, and that operating profit is used as the basis for those cash flows. The discounting, terminal growth and comparison against carrying amount are assumed to be performed by PLC outside the tool.

**Validation observation.** Beyond confirming that the base case is used, the owner has not clarified how the DQM supports the Value in Use exercise. MRM has not been able to confirm which asset or CGU is tested, which outputs and tab are provided to PLC, whether adjustments are made outside the tool (for example, to convert operating profit into cash flows or to exclude future restructuring and enhancement costs, as IAS 36 requires), and whether the base case used is the same as for the ICARA.

### 3.3 Users and Downstream Dependencies

The DQM is owned by the Head of Finance Wealth (UKEW) and is used within the Finance function. Its outputs feed the ICARA capital and liquidity planning process, the annual Value in Use exercise undertaken by PLC, and the monitoring of HWAM's performance against the Bank's growth ambition. \[Confirm whether outputs feed any other models, DQMs or reports.\]

### 3.4 Materiality

The materiality of the DQM was assessed as High at the identification stage, based on information submitted by the owner. This assessment remains subject to review and confirmation by Model Risk Management. The classification of the tool as a DQM is assessed in Section 4.

## 4. Inventory Attestation and Classification

### 4.1 Inventory Record Accuracy

The inventory record for the Business Forecast Model reflects the information provided by the owner during the model identification phase. The record classifies the tool as a model and assigns a materiality of High. Beyond these fields, the record contains limited information on the tool's purpose, use, inputs and outputs. Following the classification assessment in Section 4.2, the inventory record requires updating to reflect the tool's classification as a DQM. \[Insert finding reference if the incomplete record is raised in Section 7.\]

### 4.2 DQM vs Model Classification Assessment

During the identification phase, the owner classified the Business Forecast Model as a model. Following discussions with the owner and a review of the Excel file, Model Risk Management has reassessed this classification against the Bank's \[insert policy name\], which distinguishes models from DQMs in line with PRA SS1/23.

The tool produces forecasts and relies on expert judgement-based assumptions. Both characteristics are consistent with the SS1/23 model definition and do not, in themselves, determine the classification. The determining factor is the nature of the processing performed by the tool.

The tool does not apply statistical estimation or any statistical, economic or financial technique to derive its outputs. Assumptions are hard-coded as fixed inputs, with some recorded and briefly explained in the "Assumptions" tab of the Excel file. The tool then applies simple arithmetic calculations to these inputs. For example, in the "HWAM Base Case ICARA Scenarios" tab, yearly closing Assets under Management (AUM) are calculated as the previous year's closing AUM plus inflows, less outflows, plus or minus market performance. Market performance is calculated by applying a fixed 5% market performance assumption to Multi Asset Funds (MAF), and outflows are calculated using an assumed annual rate of customer attrition.

The tool's outputs are therefore fully determined by its inputs, and the uncertainty in the forecasts arises from the assumptions rather than from the method used to process them. On this basis, the Business Forecast Model is classified as a Deterministic Quantitative Method (DQM). Given its High materiality and the use of its outputs in ICARA capital and liquidity planning and the annual Value in Use exercise, relevant aspects of the MRM framework are applied proportionately through this review.

&#91;Open point: confirm that the other calculation types in the tool are also arithmetic applications of fixed assumptions, and that the flow multiples and attrition rates are not produced by a separate analytical process.\]

### 4.3 Ownership Confirmation

The DQM is owned by the Head of Finance Wealth (UKEW). \[Confirm whether the owner has formally accepted ownership, e.g. through the identification form or the inventory attestation.\]

## 5. DQM Specification and Implementation Assessment

### 5.1 Inputs and Data Sources

The DQM uses the following inputs, all entered manually as hard-coded values:

- **Starting AUM:** AUM as at September 2025, held in the hidden "AUM" tab and assumed to remain static until the end of 2025. The 2025 closing AUM forms the 2026 opening AUM.
- **Current-year actuals:** monthly operating P&L actuals for January to June 2026, entered as values in the "2026 P&L Revised" tab.
- **Prior-year starting points:** 2025 income and cost levels, 2025 average wages and FTE, used as the base for most income and cost lines.
- **Economic and business parameters:** inflation, salary inflation, the own cash at bank interest rate, the protection income growth rate, the bonus growth rate and IT FTE, hard-coded in the "HWAM Base Case" tabs.
- **Bank-level inputs:** total Bank customer numbers and their growth, used to drive new customer numbers.
- **Historical analysis performed outside the tool:** customer acquisition over the last two years, historical margins, prior-year customer flows, three-year fee averages and the five-year historical average return of a balanced fund. These inform the assumptions but are not held in the workbook.

The workbook comments for MAF AMC income and wealth and tax advice income refer to separate schedules, which are not held in the workbook and were not provided for this review. \[Obtain the schedules and confirm how their figures enter the workbook.\]

&#91;Add data sources, how they are extracted, and any reconciliation to the general ledger or source systems.\]

### 5.2 Calculation Logic and Assumptions

The calculations follow a single flow: customer numbers and AUM drive income, FTE drives most costs, and operating profit is total income less total costs. The annual forecast is calculated in the "HWAM Base Case ICARA Scenarios" and "Base ICARA" tabs and then phased monthly for the current year. All calculations are arithmetic applications of the assumptions described below. The "Assumptions" tab records the rationale for most assumptions, but is not linked to the calculation tabs.

**Customers and AUM**

- Multi Asset Fund (MAF) customers are split into three categories aligned with the Bank's segmentation and assigned by CON-ID: Asset Rich Grey, High Income Professionals, and Other (all remaining individuals, corporates and trusts). Flows are split between new or closed customers and existing customers.
- New Asset Rich Grey and High Income Professional customer numbers are based on acquisition over the last two years, expressed as a percentage of total Bank customers, and grow in line with Bank growth. This represents an "as is" view with no change in strategy. New customer numbers are multiplied by the historical average deposit, plus market growth, to give new customer inflows. Inflow growth rates of 0.7% (Asset Rich Grey) and 0.6% (High Income Professionals) are applied across all years. No growth is assumed for Other.
- Inflows and outflows for existing customers are based on prior-year actuals as a percentage of total brought-forward MAF AUM.
- Closing AUM for each year is calculated as opening AUM plus inflows, less outflows, plus or minus market performance. A fixed market growth assumption of 5% is applied to MAF, set as the lower of expected fund performance net of fees (5.4%) and the five-year historical average return of a balanced fund, unchanged from the prior forecast.
- Cash & Equivalents (C&E) and Segregated portfolios have no forecast flows and grow with inflation. TPD and SHB Pension balances are assumed to be fully redeemed in 2025.

**Income**

Income is forecast line by line in the "HWAM Base Case ICARA Scenarios" and "HWAM Base Case" tabs. Each line carries a short comment in the workbook describing its nature. The table combines these comments with the forecast basis described elsewhere in the workbook.

| Income line | Description | Forecast basis |
| --- | --- | --- |
| MAF AMC income | Annual management charge on HWAM Multi Asset Funds for general clients. MAF are actively managed portfolios and carry a higher yield. | Yield, based on historical margins, applied to MAF AUM. The comment refers to a separate schedule. |
| C&E AMC income | Annual management charge on non-MAF assets held under custody and administration. Custody & Execution supports the full client offering and the advisory business, and offers potential conversion into MAF. | Yield applied to C&E AUM, which has no forecast flows and grows with inflation. |
| Segregated | Investment management fees on funds managed by HWAM through discretionary mandates. | Yield applied to Segregated AUM, which has no forecast flows and grows with inflation. |
| TPD | MAF annual management charge for clients originally sourced from independent financial advisers. This is a closed channel. | No longer used. Balances were fully redeemed in 2025. |
| SHB Pension | MAF annual management charge for employees who selected HWAM funds for their pension pots. | No longer used. Balances were fully redeemed in 2025. |
| ACD fees (BONY fees) | Fund fees charged by the third-party administrator. Before Handelsbanken became the Authorised Corporate Director (ACD), fund fees were received net of these charges. | No longer used. |
| Overseas custody fee | Charges for custody and administration of overseas clients' funds. | Three-year average starting point, growing with market growth. |
| Dealing | Commission on deals executed on behalf of clients. | Three-year average starting point, growing with market growth. |
| Interest receivable | Interest received on own bank balances. | Own cash at bank interest rate applied to an assumed average balance of £15m. |
| Client interest | Interest received on client balances. | \[Confirm basis.\] |
| Wealth and tax advice | Client wealth and tax advice fees, billed on a fixed fee or time cost basis. | 2025 income increased by inflation. The comment refers to a separate schedule. |
| Protection | Commission on insurance products advised on. | Hard-coded growth rate of 35%, kept flat across all years, described as based on historical growth. |

The TPD, SHB Pension and ACD fee lines are no longer used but remain in the workbook.

**Costs**

- Salaries, employer's National Insurance and benefits are calculated as FTE multiplied by the 2025 average wage, increased by salary inflation. FTE grows with customer numbers at one CD per 150 customers and one support staff member per two CDs. Five financial crime FTE are added in 2026 to support AML work and removed in 2027.
- Bonuses start from £200k proposed to the Remuneration Committee for 2025, plus a 34.95 \[confirm unit\] uplift for tax and benefits, and grow with FTE and inflation.
- Rent and premises costs are a headcount recharge for both office locations, increased by inflation.
- Computer, communication, travel and entertainment, advertising and supplies costs are 2025 levels plus inflation. Purchased services and other internal expenses are 2025 levels plus inflation, after removing AML and system upgrade costs. One-off costs of £500k for AML remediation and £670k for system updates are forecast for 2026.
- Internal IT staff costs are calculated as hard-coded FTE multiplied by the 2025 average wage, increased by salary inflation.
- Other expenses apply 20% VAT and a 90% irrecoverable VAT rate to accounts payable costs.
- &#91;Add the basis for depreciation and impairment.\]

**Current-year phasing and actuals**

- The "Monthly Phased" tab divides the annual 2026 base case equally across the 12 months.
- The "2026 P&L Revised" tab shows the 2026 annual forecast, linked to the "HWAM Base Case ICARA Scenarios" tab, alongside the monthly operating P&L. January to June are populated with actual values; July to December use simple formulas and links to other tabs. The tab appears to be updated with actuals as they become available. \[Confirm with the owner.\]

**ICARA capital and liquidity view**

The "Monthly Phased ICARA" tab extends the current-year operating P&L into capital and liquidity measures:

- Cash at central bank is rolled forward using the monthly cashflow to give total cash movement and the cash balance.
- Wind-down amounts are calculated at 110%, 125% and 150% of a hard-coded value with no documented source. The cash balance divided by this value gives the "% over liquid assets".
- The equity balance is shown, together with wind-down as a percentage of own funds.
- A summary table feeds the "Capital Forecast 2026" chart, covering minimum requirements, own funds and liquidity under the updated base and the base case, divergence, and BRT. \[Confirm what the hard-coded wind-down value represents and what BRT refers to.\]

**Stress scenarios**

&#91;To be completed: ICARA S1 and S2 scenarios and their summaries.\]

### 5.3 Outputs and Their Use

The DQM produces the following outputs:

- **Annual P&L summary** ("Summary revised" tab): average AUM, investment and other income, external and internal costs, depreciation and impairment, total costs, operating profit and FTE for each forecast year, with annual growth rates. The 2026 figures link to the "2026 P&L Revised" tab and so combine actuals to June with the forecast for the rest of the year. Figures for 2027 onwards are the same as in the "Summary" tab, which links to the "HWAM Base Case" tab.
- **P&L and AUM forecasts and charts:** total income, total expenses and profit before tax; AUM by MAF, C&E and Segregated; and the AUM mix.
- **Current-year monthly P&L** ("2026 P&L Revised" tab), combining actuals and forecast.
- **ICARA capital and liquidity metrics** ("Monthly Phased ICARA" tab): cash balance, wind-down amounts, own funds and liquidity against minimum requirements, and the "Capital Forecast 2026" chart.

These outputs feed ICARA capital and liquidity planning, the annual Value in Use exercise, and performance monitoring against the upside forecast. \[Confirm which tabs are used as the source for each downstream use.\]

### 5.4 Implementation Testing

&#91;To be completed: recalculation or reasonableness checks performed, and results.\]

## 6. DQM Governance

### 6.1 Roles and Responsibilities

&#91;To be completed: owner, developer, users and approver of outputs.\]

### 6.2 Documentation

No formal documentation exists for the DQM. Limited explanations of some assumptions are recorded in the "Assumptions" tab of the Excel file. \[Finding reference: Section 7.2.\]

### 6.3 Change Management and Version Control

&#91;To be completed.\]

### 6.4 Access and User Controls

&#91;To be completed.\]

### 6.5 Ongoing Monitoring

&#91;To be completed, e.g. comparison of forecasts against actuals.\]

## 7. Limitations and Findings

### 7.1 Known Limitations and Compensating Controls

&#91;To be completed: limitations acknowledged by the owner and any compensating controls.\]

### 7.2 Findings and Recommendations

The absence of documentation is confirmed as a finding. Other rows are candidates to be confirmed or removed.

| ID | Finding | Status | Severity | Recommendation | Owner | Due date |
| --- | --- | --- | --- | --- | --- | --- |
| F1 | No formal documentation exists for the DQM. | Confirmed | \[TBC\] | \[TBC\] | Head of Finance Wealth (UKEW) | \[TBC\] |
| F2 | Inventory record is incomplete and classifies the tool as a model. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |
| F3 | Assumptions are hard-coded and only partially documented, with largely qualitative rationales. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |
| F4 | Customer mapping to segmentation has not been refreshed; previous forecast metrics are reused. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |
| F5 | The "Assumptions" tab is not linked to the calculation tabs, so the documented assumptions can diverge from the values actually used. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |
| F6 | The workbook contains near-identical tabs that feed different outputs (e.g. "HWAM Base Case" feeds the summary tabs, while "HWAM Base Case ICARA Scenarios" feeds the current-year P&L), creating a risk of inconsistent outputs if one tab is updated and the other is not. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |
| F7 | Key inputs are hard-coded without a documented source, including the wind-down value in "Monthly Phased ICARA" and the hidden "AUM" tab. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |
| F8 | Some assumptions refer to past periods (e.g. the 2025 bonus starting point), and may not have been refreshed for the current forecast. Income lines no longer in use (TPD, SHB Pension and ACD fees) remain in the workbook. | Candidate | \[TBC\] | \[TBC\] | \[TBC\] | \[TBC\] |

## 8. DQM Risk Rating

&#91;Insert rating using the Bank's DQM rating scale.\]

### 8.1 Rating Rationale

&#91;To be completed, drawing on materiality (Section 3.4) and findings (Section 7.2).\]

## 9. Review Conclusions and Next Review

### 9.1 Conclusion

&#91;To be completed.\]

### 9.2 Next Review Date or Trigger

&#91;Insert next review date per the Bank's DQM review frequency, and any events that would trigger an earlier review.\]

## Appendices

### Appendix A: Documents Reviewed

- DQM identification form, completed by the owner.
- Business Forecast Model Excel file (tabs listed in Section 3.1).
- &#91;Add any other documents or evidence.\]

### Appendix B: Testing Details

&#91;To be completed.\]
