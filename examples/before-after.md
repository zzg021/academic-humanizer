# Editing examples for methodological and simulation papers

All passages and numerical values below are constructed illustrations. They are
not findings from the reference papers. Each revision uses only information in
its input. Editorial commentary is separate from manuscript text.

## 1. Tighten expression while preserving the comparison

**Before**

> It is worth noting that, in the condition with 30 clusters and a cluster size of
> 20, Method A had a coverage rate of .91, whereas Method B had a coverage rate of
> .95. This comparison was based on 1,000 replications for nominal 95% confidence
> intervals. These results are for normally distributed indicators only.

**After**

> With 30 clusters and a cluster size of 20, coverage was .91 for Method A and .95
> for Method B. The comparison used 1,000 replications and nominal 95% confidence
> intervals, with normally distributed indicators only.

**Editorial note:** Removed empty emphasis and repetition. Retained the interval
type, nominal level, replication count, and distributional restriction. No test of
the difference or claim about other conditions was added.

## 2. Reorder paragraphs to connect the question to the design

**Before**

> We used 1,000 replications per condition. We varied cross-loading magnitude and
> sign. Factor correlations were the target quantities, and we evaluated their
> bias and interval coverage.
>
> Our question was whether a fit-based model choice identified the model with
> better factor correlation recovery. A model can meet a fit criterion while
> providing biased estimates of a target parameter. We compared model choices
> based on fit with factor correlation recovery across the design conditions.

**After**

> A model can meet a fit criterion while providing biased estimates of a target
> parameter. We asked whether a fit-based model choice identified the model with
> better factor correlation recovery.
>
> We varied cross-loading magnitude and sign, using 1,000 replications per
> condition. Factor correlations were the target quantities, and we evaluated
> their bias and interval coverage. We compared model choices based on fit with
> factor correlation recovery across the design conditions.

**Organization note:** Moved the rationale and question before the design.
Retained every design detail and the comparison. The revision does not assert
that the hypothesized discrepancy actually occurred.

## 3. Flag missing evidence without supplying it

**Input**

> Our estimator was more robust than the alternatives when indicators were skewed.

**Review comment**

> "More robust" does not identify the performance measure, comparison methods, or
> skewness conditions. The supplied passage contains no supporting result. Please
> identify the relevant results and clarify whether robustness refers to bias,
> coverage, convergence, or another criterion. I have retained the claim pending
> that clarification.

**Editorial note:** No invented table, effect size, test, or narrower substantive
claim. A polished final sentence requires the missing information.

## 4. Make a change in inferential strength visible

**Input**

> In the simulation, absolute bias was smaller for Method A than Method B at sample sizes
> of 100 and 200. This proves that Method A is unbiased in all samples.

**Substantive proposal**

> In the simulation, absolute bias was smaller for Method A than Method B at sample sizes
> of 100 and 200. These results favor Method A on absolute bias under the conditions examined.

**Reason:** Smaller simulated absolute bias does not establish zero bias or a claim about
all samples. The proposed revision narrows the interpretation and must be reported
as substantive. With copyediting-only authorization, retain the original claim
and attach this concern; do not silently substitute the alternative.

## 5. Preserve a theoretical claim and its mathematical condition

**Before**

> It is worth emphasizing that Proposition 1 proves consistency under Assumptions
> A1–A4. The proof requires $n \to \infty$ with the number of indicators fixed
> \citep{example_theory}.

**After**

> Proposition 1 proves consistency under Assumptions A1–A4. The proof requires
> $n \to \infty$ with the number of indicators fixed \citep{example_theory}.

**Editorial note:** Retained "proves," the technical meaning of consistency, the
assumptions, equation, and citation key. The theorem itself was not verified from
this excerpt. The citation key is illustrative, not a real reference to add.

## 6. Keep failure information and interval interpretation visible

**Before**

> Among the 940 converged fits from 1,000 attempted replications, the 95% credible
> intervals had coverage of .93. We excluded the remaining fits from this summary.
> It should be noted that this is a summary among converged fits.

**After**

> Among the 940 converged fits from 1,000 attempted replications, the 95% credible
> intervals had coverage of .93. The remaining fits were excluded from this summary.

**Editorial note:** Removed a repeated qualification while retaining the
denominator, exclusions, and credible-interval label. The .93 is a simulated
coverage rate, not a posterior probability. If relevant to the interpretation,
flag whether the failure pattern and Monte Carlo uncertainty were examined;
do not add unreported diagnostics or computed values during a prose edit.
