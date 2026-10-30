**Model Performance, Accuracy and Stability**

*Description*

As part of the annual refresh, the SAA framework includes a materiality assessment, which compares the newly optimised allocations with those of the prior year. The prior-year results are carried into the current SAA Output file, where a "Change" tab sets out the year-on-year movement in allocations for each strategy.

Two measures are used to assess whether the proposed changes are material:

- **Absolute sum of changes.** This aggregates the absolute differences between the proposed and prior-year weights and compares the total with a materiality threshold. The threshold is currently set at the ex-ante standard deviation referenced in the 2022 SAA review document. The instructions note that the threshold should be re-evaluated each year.
- **Tracking error.** This estimates the ex-ante tracking error of the proposed allocation relative to the prior-year allocation, using the matrix taken from the SAA Model file.

Where a strategy's proposed changes do not meet the materiality threshold, its allocation is reset to the prior-year weights and the simulation stage is re-run. Through this mechanism the framework limits allocation changes that are not material, and so promotes year-on-year stability in the strategies. The practical steps, including the transfer of inputs between workbooks, are described in the Model Implementation section and are not repeated here.

*UKRM Independent Assessment*

The SAA model is a portfolio construction tool rather than a forecasting model. Its performance therefore cannot be assessed through conventional backtesting of predictions against realised outcomes. UKRM considers that performance should instead be judged against the model's design objectives:

- that each strategy achieves its intended risk level relative to the others;
- that allocations remain diversified; and
- that outputs are stable and reproducible given the inputs.

On this basis, the relevant evidence would include:

- comparison of realised strategy volatility and returns against the ex-ante targets and projected ranges;
- analysis of how sensitive the optimised weights are to changes in the inputs; and
- confirmation that the optimisation and simulation produce consistent results across repeated runs.

The materiality assessment addresses one dimension of stability, namely the year-on-year change in allocations. It does not, however, show whether a given allocation is robust to reasonable changes in inputs, or whether the optimiser reliably converges to the same solution. No sensitivity analysis of the optimised weights to the expected return, volatility or correlation assumptions was provided. This is a recognised limitation of mean-variance optimisation, in which small changes in expected returns can produce large changes in weights. The use of composite indices mitigates this risk in design, but no evidence was provided to show its effect in practice.

Similarly, no evidence was provided on the stability of the optimiser or the simulation. The instructions require an initial optimisation of 500 iterations followed by a second of 1,000 iterations to ensure that a global maximum is found. However, no testing was presented to show that repeated runs produce consistent weights, or that the 10,000-iteration Monte Carlo simulation produces stable projected characteristics.

UKRM did not have access to the @RISK add-in. Consequently, UKRM could not re-run the optimisation or the simulation, test alternative settings or constraints, or perform independent sensitivity or convergence testing. The assessment in this section therefore relies on the outputs produced by the developer and on a static review of the model files and macros. The conclusions above should be read in that light.

Overall, the materiality assessment is a reasonable control over year-on-year changes in allocations. However, the performance, accuracy and stability of the model are asserted rather than evidenced. UKRM considers that these gaps are best addressed through the ongoing monitoring plan, which should include outcomes analysis, sensitivity testing and convergence checks.

---

Earlier in the project you found that B57:J66 in the SAA Model holds the correlation matrix, not a covariance matrix. If that applies to the tracking error input, it would affect the tracking error figures. It may be worth either referencing it here or confirming the implementation section already covers it.
