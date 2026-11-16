# Methodological safeguards

Use the checks relevant to the passage. Flag substantive concerns separately from
prose edits, with the specific sentence and the information needed to resolve them.
These checks help preserve scientific meaning; they do not prescribe a universal
simulation design or replace statistical review.

## Quantities, models, and claims

- Distinguish a population quantity or estimand from an estimator, a realized
  estimate, and a summary across replications. An estimate's observed error is not
  automatically evidence of estimator bias.
- Keep model assumptions, identification conditions, derived results, and empirical
  findings distinct. Preserve theorem assumptions and mathematical qualifiers;
  finite-sample simulation results do not establish an asymptotic property.
- Preserve the scale and level of a quantity: standardized versus unstandardized,
  conditional versus marginal, within-cluster versus between-cluster, and observed
  versus latent. Explain a switch when the manuscript supplies its rationale.
- Retain the distinction between association, prediction, and a causal effect.
  Changes between these interpretations require a substantive proposal.
- Keep statistical significance, effect magnitude, and practical importance
  distinct. Do not add a test or a p-value to justify a comparison.

## Simulation design and reporting

Trace the argument from question to design to evaluation to conclusion. When a
necessary link is unclear, identify it without inventing a design choice.

- Identify the target quantity, data-generating process, fitted models or methods,
  manipulated factors, fixed features, and performance measures. Distinguish a
  generating parameter from a fitted-model constraint and from an estimated value.
- Preserve the distinction between sample size, number of clusters, cluster size,
  number of replications, and number of design conditions. In Bayesian work,
  distinguish simulation replications from chains, draws, and effective sample size.
- Keep population calculations separate from summaries of repeated samples.
  Explain how they complement each other when that connection is supplied.
- Clarify which factors are crossed and which comparisons hold other features
  fixed. State interactions and exceptions when they matter to the conclusion.
  Do not replace condition-specific findings with an unqualified overall ranking.
- Keep the evaluation denominator visible: all attempted replications, converged
  fits, admissible solutions, or another stated subset. Preserve exclusions and
  failure rates; a summary among successful fits may describe a selected subset.
- Flag an unclear definition of bias, relative bias, RMSE, empirical sampling
  variability, average estimated standard error, coverage, rejection rate, or power.
  Preserve the manuscript's verified definitions. Distinguish signed bias from
  its magnitude; a smaller signed value need not be closer to zero. Relative bias
  needs particular care when the target quantity is zero or near zero.
- Distinguish uncertainty from finite simulation replications (Monte Carlo
  uncertainty) from sampling variability, estimated standard errors, and posterior
  uncertainty. If a conclusion depends on small simulated differences and Monte
  Carlo uncertainty is unavailable, flag that limitation without supplying a value.
- Preserve how summaries were formed across replications and across conditions,
  including weights, aggregation rules, and thresholds. A range and an average
  answer different questions; choose neither automatically.

## Psychometric interpretation

- Keep constructs, indicators, scores, latent variables, and their model-based
  representations distinct. Preserve the manuscript's interpretation of an
  aggregate, including formative or reflective meanings when relevant.
- Distinguish measurement error, sampling error in an aggregate, and model
  misspecification. Do not substitute one explanation for another to shorten text.
- Keep global model fit, parameter recovery, measurement invariance, and the
  validity of a proposed score interpretation distinct. Evidence about one does
  not automatically support a claim about the others.
- Preserve the exact type of invariance, the constrained parameters, the comparison
  model, and the criterion used. Treat fit-index cutoffs and labels such as
  "negligible" as conditional or attributed judgments, not universal facts.
- Keep measurement and structural components separate where that distinction
  explains a result. Preserve whether a reported discrepancy concerns loadings,
  intercepts, residuals, correlations, regression coefficients, or latent means.

## Bayesian and frequentist interpretation

- Preserve confidence versus credible intervals and their stated interpretations.
  Keep nominal interval level, observed simulation coverage, interval width, and
  posterior probability distinct.
- Preserve the roles of priors, likelihood, posterior summaries, and model checks.
  A prior's informativeness depends on scale and parameterization; do not silently
  relabel a prior as weakly informative or noninformative.
- Distinguish evidence of convergence or computational adequacy from evidence of
  parameter recovery or model adequacy. Retain caveats about diagnostics and failures.
- Treat substantive claims in reference papers as claims to evaluate in context.
  Their role as writing references does not settle a methodological disagreement.

## Evidence and manuscript mechanics

Use an evidence pointer only after checking that the supplied figure, table,
equation, or reference supports the particular claim. A citation's presence alone
does not establish support; if its contents are unavailable, say so. Preserve
citations and flag questionable support rather than silently deleting or replacing
them. Do not add a claim to match a convenient citation.

In LaTeX or Quarto, preserve commands, labels, cross-references, citation keys,
mathematical environments, code chunks, and executable expressions. Move prose
without breaking their scope. Edit analysis code or generated results only when
that work is separately requested.
