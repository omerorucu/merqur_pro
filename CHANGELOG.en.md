# MerQur Pro: Changelog

## 3.4.0 (2026-11): Accuracy and validation; MerQur 2.5.0 base

> "Societies that wish to live in comfort without working, without tiring and without producing are doomed to lose first their dignity, then their freedom, and then their independence and their future."
> — Mustafa Kemal Atatürk

- MerQur Pro 3.4.0 brings the accuracy and validation improvements of the free MerQur 2.5.0: result values are stored at full precision and very small values are printed with significant digits.
- Errors affecting results in specific data situations were fixed in data loading, probit (natural response), GLMM/GEE, cointegration and Cox regression.
- New options were added to panel regression, mixed models, MANOVA, ARIMA, Cox and robust regression, the Dunn test, machine learning and multiple imputation (off by default); multi-group confirmatory factor analysis and measurement invariance are faster.
- The template library is unchanged (211 templates); minor improvements were made to texts and stability.

## 3.3.0 (2026-11): 16 new templates: forest tree breeding and quantitative genetics, quality, time series; MerQur 2.4.1 base

> "Societies that wish to live in comfort without working, without tiring and without producing are doomed to lose first their dignity, then their freedom, and then their independence and their future."
> — Mustafa Kemal Atatürk

- 16 new templates (211 in total), each compared with published results and, where an equivalent exists, with SAS:
  - Forest tree breeding and quantitative genetics:
    - provenance–progeny trial: variance components; individual and family-mean heritabilities with standard errors; coefficients of variation; genetic correlation and its standard error from bivariate REML; type B correlation for traits measured on different individuals; a model for unreplicated trials;
    - selection gain and selection indices (Smith–Hazel, restricted index, Pesek–Baker desired-gains index);
    - QST–FST comparison;
    - genetic diversity in seed orchards and breeding populations (fertility variation, effective number of parents, status number, pollen contamination, effect of thinning);
    - clonal and multi-site progeny trials (broad-sense heritability, type B genetic correlation, age–age correlation).
  - Quality: multivariate control chart (Hotelling T², PCA-based T² and SPE monitoring, contribution decomposition); non-normal process capability (percentile/Clements, Weibull, lognormal, gamma, Johnson, Box-Cox).
  - Time series and econometrics: structural VAR (A/B restrictions, Blanchard–Quah long-run identification, structural impulse responses, FEVD); extended GARCH (GARCH-M, IGARCH, GJR/TGARCH, APARCH, EGARCH, NAGARCH; normal, t, GED); panel count models (fixed- and random-effects Poisson and negative binomial, Hausman test).
  - Mixed models and survival: factor analytic mixed model (multi-environment trials, genotype × environment); GEE for ordinal and nominal responses; discrete-time survival model (person-period data, logit/cloglog).
  - Multivariate and causal: resampling-based multiple testing (Westfall–Young maxT and minP); social network analysis (centrality, density, community detection); causal graph (DAG) analysis (adjustment sets, instrumental variables, testable conditional independencies).
- Futility boundary option in the group sequential design template (binding and non-binding β-spending).
- Genetics example data: the example data of five genetics templates were replaced with an openly licensed (CC0) Cilician fir (Abies cilicica) microsatellite dataset; the templates were re-validated against published values for these data.
- Fix: in non-normal process capability, the Johnson SB distribution now takes a cumulative probability of 0 or 1 for observations outside its support instead of stopping with an error.
- All analyses and fixes from the free MerQur 2.4.0 and 2.4.1: six new analyses (Gamma/Inverse Gaussian/Tweedie GLM, relative risk and prevalence ratio, complex-sample ordinal and multinomial logistic regression, tolerance intervals, ANOM), the Randomization Plan tool, reading of decimal-comma numbers and numbers stored as text; fixes to Variance Components and to two-way ANOVA, ANCOVA and crossed mixed models with empty cells.

## 3.2.0 (2026-11): STM, variety registration templates, MerQur 2.3.2 base

> "Societies that wish to live in comfort without working, without tiring and without producing are doomed to lose first their dignity, then their freedom, and then their independence and their future."
> — Mustafa Kemal Atatürk

- New template: structural topic model (STM); topics from a text column, topic prevalence and content with covariates, K selection, representative documents, effect plots, topic network.
- New: five templates for variety registration (DUS and VCU): combined over-years distinctness (COYD; long-term, MJRA, 2×1%, decision schemes), combined over-years uniformity (COYU; relative variance), uniformity by off-types (single and two-stage tests, OC curve), GAIA phenotypic distance, and the location × year combined randomized complete block analysis (fixed/random effects, Satterthwaite and REML, EMMs, LSD, letter groups). Validated against the worked examples of UPOV TGP/8/5 and SAS (195 templates in total).
- Language-aware decimal separator in template output; template fixes; SAS equivalents for 14 templates.
- Fixes from the free MerQur 2.3.2: options that cannot be applied are now reported with the reason, and convergence warnings are visible.
- Exploratory factor analysis, oblique rotation: the rotation sums-of-squares column is labelled diag(ΦP′P), the structure-matrix sums of squares (ΣS²) are added next to it, and the "cannot be added" note appears only for oblique rotations. Numbers are unchanged.
- MANOVA (crossed design): when the computation fails, the actual reason (empty cell, singular design matrix, insufficient error degrees of freedom) is stated.

## 3.1.0 (2026-11): 24 new templates, parameter window, citations

### New

- **24 new validated templates (189 in total).**

  - Econometrics: ARDL/NARDL bounds test, structural-break unit roots (Zivot–Andrews, Lee–Strazicich) and Toda–Yamamoto, second-generation panel tests (Pesaran CD, CIPS, Pedroni, Kao, Dumitrescu–Hurlin, CCE/AMG), stochastic frontier analysis, data envelopment analysis and Malmquist index, discrete choice (mixed, nested and latent-class logit, WTP).

  - Clinical: clinical prediction models (restricted cubic splines, bootstrap validation, calibration, decision curves, nomogram), penalized Cox, RMST regression, crossover trials, bioequivalence and non-compartmental analysis, joinpoint and interrupted time series.

  - Meta-analysis, SEM and design: proportion meta-analysis (GLMM by default), RI-CLPM and latent change scores, distribution fitting, robust ANOVA, mixture experiments, diallel/line × tester/augmented blocks/Latin squares.

  - Genetics, ecology and spatial: AMOVA with DNA sequences and pairwise ΦST, Bayesian phylogenetics with MrBayes, DNA barcoding and species delimitation, sequence alignment (optional GenBank), occupancy and capture–recapture models, spatio-temporal kriging.

  - Each was compared with a published source and, where an equivalent exists, with SAS.

- **Parameter settings window.** All variables and options of a template are set in Variables, Model, Options, Advanced and Output tabs; **OK and run** runs the analysis with these settings. A short summary remains in the side pane; double-clicking a template opens the window.

- **All parameters in every template.** The meaningful options of the underlying method were added to the existing 165 templates (8 → 13.5 parameters per template on average). With default settings, results are identical to before.

- **MrBayes 3.2.9 is included** (GNU GPL v3, separate program; license and source code in the installation folder). Template summaries were compared with MrBayes's own sump/sumt output.

- **Software and citations.** Every code and template run lists MerQur Pro, R/Python and the packages used with their versions and official citations; the section stays in the report even with the code appendix turned off. Re-running a `.mqs` script with different package versions shows a warning.

- **Help → Check for updates.** Runs only when clicked; no network request at start-up.

### Changed

- The AI **code assistant was removed.** The AI Interpreter for results and reports remains. The "generated with AI" flag in older `.mqs` scripts is still read.

- License agreement PRO-1.1.0: code-assistant clauses removed, update check and MrBayes notice added. It is accepted once more on first start.

- `uzay_zaman_kriging` is now true spatio-temporal kriging; the former cokriging template is now `es_kriging` (results unchanged).

### Fixed

- Very small decimal values such as 1e-14 were rounded to 0 in the template form.

- Some template options produced raw errors or showed Turkish column names in the English interface (every option was checked one by one). In `cift_engel`, the bc and ihs distributions were removed because of a package bug.

## 3.0.0 (2026-10-31): first release

Base version: MerQur 2.3.1 (all analyses and fixes of the free edition included).

### New

- **Code tab.** Run code with embedded Python 3.13 and your installed R 4.5.x, or optionally your own Python interpreter. The active dataset is available as `df`. Tables, figures and text become cards in the Results, Table, Chart and Report tabs, go into the DOCX report with their code, and are saved with the `.mqr` project.

- **Safe execution.** Code runs in a separate worker process. Cancel stops it within a second, the time limit is configurable, and the main window survives a crashed worker. Syntax errors are highlighted on their line. Missing packages come with `install.packages(...)` / `pip install ...` suggestions. A run history is kept.

- **165 ready templates in 23 categories** (139 R, 26 Python). Each template has a parameter form, sample data and sample parameters. Templates were validated against the source package and published examples. Where an equivalent SAS procedure exists, its code is shown for comparison. "Save as template…" adds personal templates. The template tree has a search box.

- **Multilingual template output.** Text output, table column names and cells, code comments and SAS equivalents are shown in the interface language (Turkish, English, Spanish).

- **`mq` module.** Call MerQur's analysis engines from code (`mq.ttest`, `mq.mediation` and 12 more wrappers, `mq.calistir`, `mq.yardim`). `mq.veriye_yaz` writes new columns or filtered rows to the Data tab after a confirmation dialog, and the change can be undone.

- **AI code assistant.** Generates code from a Turkish or English request, explains errors with the fix shown as a diff, and interprets output. The AI Interpreter is also enabled in Pro. It works with your own API key. Data cells are never sent.

- **`.mqs` code steps.** The GUI asks for approval for each code step. Headless runs execute code steps only with `--kod-izin`.

- **License.** Personal, one-year, offline-verified license key. The holder's name and institution appear in the About window and in the report footer. MerQur Pro has its own license agreement (EULA-PRO), and commercial use is permitted.

- **Side-by-side installation.** Runs next to the free MerQur with its own folder, settings, recent files and icon. On first start, the language, theme, font size, chart DPI and AI provider settings of the free edition are copied once.

- The program makes no network requests on its own. There is no update check.

### Verification

- Smoke test on the built program: 165/165 templates ran with their sample data. The Python and R code tabs, `.mqs` code steps (with and without permission) and the absence of network requests were checked.

- Code-tab robustness scan: 1199 runs, 0 raw exceptions.

- The installer and the program are code-signed by Ömer Kamil Örücü.

