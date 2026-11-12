# Business Forecast Model – DQM Review Report

Nov 4, 2026 · @Ariel Gimenez

## 1. Executive Summary

### 1.1 Purpose of the Review

This report sets out the first review by Model Risk Management of the Business Forecast Model, an Excel-based tool used to produce five-year forecasts for the Wealth and Asset Management (WAM) division. \[To be completed.\]

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
- A review of the Excel file, including the "WAM Base Case ICARA scenario" and "Assumptions" tabs.

&#91;Add any testing performed, e.g. recalculation or reasonableness checks.\]

## 3. DQM Overview, Use and Intended Purpose

### 3.1 DQM Description

The Business Forecast Model is an Excel-based tool that produces five-year forecasts of the profit and loss (P&L) of the Bank's Wealth and Asset Management (WAM) division, together with other business forecasts. The tool is maintained in two versions that share the same structure and calculation logic and differ only in their underlying assumptions:

- **Base case forecast**, which represents the expected business outlook.
- **Upside forecast**, which reflects the Bank's growth ambitions for the WAM division.

The understanding set out in this report is based on discussions with the DQM owner, the identification form completed by the owner, and a review of the Excel file. No formal documentation was available for the DQM; this is addressed in Section 7.

### 3.2 Business Use and Intended Purpose

The DQM supports financial planning for the WAM division. Its two versions serve distinct purposes:

- The base case forecast is used for ICARA capital and liquidity planning, and for the Bank's annual Value in Use exercise.
- The upside forecast is used as a benchmark against which WAM's actual performance is assessed.

The DQM is run quarterly. \[Add examples of the other business forecasts produced, if they have separate uses.\]

### 3.3 Users and Downstream Dependencies

The DQM is owned by the Head of Finance Wealth (UKEW) and is used within the Finance function. Its outputs feed the ICARA capital and liquidity planning process, the annual Value in Use exercise, and the monitoring of WAM's performance against the Bank's growth ambitions. \[Confirm whether outputs feed any other models, DQMs or reports.\]

### 3.4 Materiality

The materiality of the DQM was assessed as High at the identification stage, based on information submitted by the owner. This assessment remains subject to review and confirmation by Model Risk Management. The classification of the tool as a DQM is assessed in Section 4.

## 4. Inventory Attestation and Classification

### 4.1 Inventory Record Accuracy

The inventory record for the Business Forecast Model reflects the information provided by the owner during the model identification phase. The record classifies the tool as a model and assigns a materiality of High. Beyond these fields, the record contains limited information on the tool's purpose, use, inputs and outputs. Following the classification assessment in Section 4.2, the inventory record requires updating to reflect the tool's classification as a DQM. \[Insert finding reference if the incomplete record is raised in Section 7.\]

### 4.2 DQM vs Model Classification Assessment

During the identification phase, the owner classified the Business Forecast Model as a model. Following discussions with the owner and a review of the Excel file, Model Risk Management has reassessed this classification against the Bank's \[insert policy name\], which distinguishes models from DQMs in line with PRA SS1/23.

The tool produces forecasts and relies on expert judgement-based assumptions. Both characteristics are consistent with the SS1/23 model definition and do not, in themselves, determine the classification. The determining factor is the nature of the processing performed by the tool.

The tool does not apply statistical estimation or any statistical, economic or financial technique to derive its outputs. Assumptions are hard-coded as fixed inputs, with some recorded and briefly explained in the "Assumptions" tab of the Excel file. The tool then applies simple arithmetic calculations to these inputs. For example, in the "WAM Base Case ICARA scenario" tab, yearly closing Assets under Management (AUM) are calculated as the previous year's closing AUM plus inflows, less outflows, plus or minus market performance. Market performance is calculated by applying a fixed 5% market performance assumption to Multi Asset Funds (MAF), and outflows are calculated using an assumed annual rate of customer attrition.

The tool's outputs are therefore fully determined by its inputs, and the uncertainty in the forecasts arises from the assumptions rather than from the method used to process them. On this basis, the Business Forecast Model is classified as a Deterministic Quantitative Method (DQM). Given its High materiality and the use of its outputs in ICARA capital and liquidity planning and the annual Value in Use exercise, relevant aspects of the MRM framework are applied proportionately through this review.

&#91;Open point: confirm that the other calculation types in the tool are also arithmetic applications of fixed assumptions, and that the flow multiples and attrition rates are not produced by a separate analytical process.\]

### 4.3 Ownership Confirmation

The DQM is owned by the Head of Finance Wealth (UKEW). \[Confirm whether the owner has formally accepted ownership, e.g. through the identification form or the inventory attestation.\]

## 5. DQM Specification and Implementation Assessment

### 5.1 Inputs and Data Sources

&#91;To be completed.\] Notes gathered so far:

- The starting point of the current forecast is AUM as at September 2025, assumed to remain static until the end of the year.
- &#91;Add data sources, how they are obtained, and any manual steps.\]

### 5.2 Calculation Logic and Assumptions

&#91;To be completed.\] Notes gathered so far:

- Yearly closing AUM = previous year's closing AUM + inflows − outflows ± market performance.
- Market performance applies a fixed 5% assumption to Multi Asset Funds (MAF).
- Outflows are based on an assumed annual rate of customer attrition.
- Assumptions are hard-coded. Some are recorded and briefly explained in the "Assumptions" tab; rationales are largely qualitative and vary in level of detail.
- The Business Flows assumption reuses the metrics from the previous forecast, as the customer mapping to relevant segmentation has not been refreshed.

### 5.3 Outputs and Their Use

&#91;To be completed: outputs produced, frequency, and where they are used.\]

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
- Business Forecast Model Excel file, including the "WAM Base Case ICARA scenario" and "Assumptions" tabs.
- &#91;Add any other documents or evidence.\]

### Appendix B: Testing Details

&#91;To be completed.\]
