<div align="center">

<img src="icon/MerQurPro_icon_256.png" alt="MerQur Pro" width="160" />

# MerQur Pro

### *Analysis beyond the form: validated templates, code and the MerQur engine in one place*

**ANALYZE · MODEL · INTERPRET · REPORT**

*İNCELE · MODELLE · YORUMLA · RAPORLA*

**Integrated Academic Data Analysis & Reporting Platform: licensed edition**
*by Ömer K. Örücü*

---

![Version](https://img.shields.io/badge/version-3.5.0-5B21B6?style=flat-square)
![Base](https://img.shields.io/badge/base%20MerQur-2.5.0-7C3AED?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue?style=flat-square)
![Languages](https://img.shields.io/badge/i18n-TR%20%7C%20EN%20%7C%20ES-success?style=flat-square)
![Templates](https://img.shields.io/badge/validated%20templates-212%20in%2024%20categories-5B21B6?style=flat-square)
![License](https://img.shields.io/badge/license-commercial%20key%20required-orange?style=flat-square)

**[⬇ Download MerQur Pro 3.5.0 for Windows](https://github.com/omerorucu/merqur_pro/releases/latest)**

</div>

---

## 🔍 What is MerQur Pro?

**MerQur Pro** is the licensed edition of [MerQur](https://github.com/omerorucu/merqur). It contains
**everything in MerQur 2.5.0** (143 form-based analyses, 7 map methods, APA 7 reports) and adds
**212 validated analysis templates** and a **Code tab** for analyses that a form cannot express:
advanced econometrics, clinical prediction, phylogenetics, forest tree breeding, custom models, simulations and more.

Every template opens with a **parameter window** that exposes all meaningful options of the underlying
method. Its results become cards in MerQur's **Results, Table, Chart and Report** tabs, go into the DOCX
report with a **"Software and citations"** section, and are saved with the project.

<div align="center">

| **212** | **24** | **2 935** | **APA 7** |
|:---:|:---:|:---:|:---:|
| Validated<br>templates | Template<br>categories | Adjustable<br>parameters | Reports with software<br>citations |

</div>

MerQur Pro installs **side by side** with the free MerQur: separate folder, settings, recent files and
Start-menu icon. Installing or removing one does not affect the other.

---

## ✨ What Pro adds

### 📚 Template library: 212 validated analyses
- Each template was **validated against a published source** (package vignette, textbook table or article)
  and, where an equivalent procedure exists, **against SAS** (typical differences 1e-6 to 1e-12). Where R
  and SAS define a quantity differently, the template states which definition it uses.
- **Parameter settings window** (or double-click a template): variables and options are arranged in
  tabs (**Variables, Model, Options, Advanced, Output**) covering all meaningful options of the method;
  **OK and run** runs the analysis with these settings.
- Sample data and sample settings for every template; output fully translated (TR / EN / ES: text,
  tables, comments, SAS equivalents).

| Category | # | Examples |
|---|:---:|---|
| Genetics & genomics | 32 | provenance–progeny trials, heritability and genetic correlations, selection indices, QST–FST, seed orchard diversity, clonal and multi-site trials, AMOVA (genotypes and DNA sequences, ΦST), Bayesian phylogenetics with MrBayes, DNA barcoding and species delimitation, sequence alignment, haplotype networks, neutrality tests, GWAS, QTL mapping |
| Causal inference & panel econometrics | 18 | double machine learning, AIPW, TMLE, synthetic control, staggered DiD, regression discontinuity, second-generation panel tests (CD, CIPS, Pedroni, Kao, Dumitrescu–Hurlin, CCE/AMG) |
| Regression & efficiency models | 17 | stochastic frontier analysis, data envelopment analysis and Malmquist index, discrete choice (mixed, nested, latent-class logit, WTP), distribution fitting, robust ANOVA, beta regression, hurdle |
| Time series | 16 | structural VAR, extended GARCH, ARDL / NARDL bounds test, structural-break unit roots, Toda–Yamamoto, joinpoint and interrupted time series, ARFIMA, DCC-GARCH |
| Mixed models | 15 | factor analytic models for multi-environment trials, bioequivalence and non-compartmental PK analysis, ordinal mixed models, glmmTMB families, nlme |
| Survival | 14 | clinical prediction models (TRIPOD: splines, bootstrap validation, calibration, decision curves, nomogram), penalized Cox, RMST regression, multi-state models |
| Multivariate | 11 | Westfall–Young resampling tests, Bayesian networks, compositional and functional data |
| Psychometrics | 10 | network psychometrics, cognitive diagnosis, many-facet Rasch, DIF |
| Structural equation models | 9 | RI-CLPM and latent change scores, Bayesian SEM, ESEM, growth mixture |
| Design of experiments | 13 | variety registration (DUS and VCU), crossover trials, mixture experiments, diallel and line × tester, augmented blocks, Latin squares |
| Meta-analysis | 8 | proportion meta-analysis (GLMM), network, multivariate and multilevel meta-analysis |
| Spatial | 8 | spatio-temporal kriging, cokriging, MGWR, areal Bayesian CAR, point processes |
| Ecology | 6 | community-weighted means along environmental gradients (trait CWM, row/column/max permutation tests, Tukey letter groups), occupancy and N-mixture models, capture–recapture, diversity, PERMANOVA and dispersion (PERMDISP) |
| Quality, resampling, survey, smoothing, Bayesian, simulation, missing data, extreme values, method comparison, text | 33 | multivariate control charts, non-normal process capability, structural topic model, control charts, block bootstrap, raking, GAMLSS, brms, power by simulation, multilevel imputation, GEV/GPD, Deming |
| Starters | 2 | empty Python and R templates |

**MrBayes 3.2.9 is included**: Bayesian phylogenetic analyses run with the bundled MrBayes; nothing else to install.

### 🧾 Software and citations, for your methods section
Every run lists the software used, ready to paste into a paper: MerQur Pro, the R or Python version, and
every package used **with its version and its official citation** (and MrBayes when it was run). The
section stays in the report even when the code appendix is turned off. The package versions are also
stored with `.mqs` scripts; re-running a script with different package versions shows a warning.

### 🧑‍💻 Code tab: Python and R
- **Embedded Python 3.13** with numpy, scipy, pandas, statsmodels, scikit-learn and matplotlib. Nothing to install.
- **R** (4.5.x) through your own R installation, detected automatically. Missing packages come with a ready `install.packages(...)` suggestion.
- **Your own Python**, if you need packages beyond the embedded set.
- The active dataset is available as **`df`** in both languages. Safe execution in a separate process, **Cancel stops it within a second**, configurable time limit, error-line highlighting, run history.

### ⚙️ MerQur engine from code
The `mq` module calls MerQur's own analysis engines from Python, for example `mq.ttest(df, "y", "g")` or
`mq.mediation(...)`, and returns exactly the text MerQur's form would produce. `mq.veriye_yaz(...)` writes
new columns or filtered rows back to the Data tab **after a confirmation dialog**, and the change can be undone.

### 🤖 AI Interpreter
Optional interpretation of results and reports with **your own API key**. Only column names and summaries
are sent, **never data cells**, and a preview shows exactly what will go out. AI features do not compute or
change results.

### 📜 Scripts (.mqs) with code steps
In the GUI each code step asks for approval; headless runs execute code steps only with `--kod-izin`.

---

## 💻 System requirements

| | |
|---|---|
| **Operating system** | Windows 10 or 11, 64-bit |
| **Disk** | about 1.5 GB |
| **Memory** | 8 GB recommended |
| **R (optional)** | R 4.5.x, needed for the R templates (185 of 212). Packages are installed from within R when a template asks for them. |
| **Internet** | not required. MerQur Pro connects only when you send an AI request or start **Help → Check for updates** yourself. |

macOS and Linux builds of MerQur Pro are not available yet. The free MerQur runs on all three.

---

## 📥 Installation and updates

1. Download **`MerQurPro-3.5.0-windows-x64-Setup.exe`** from the [latest release](https://github.com/omerorucu/merqur_pro/releases/latest).
2. Run the installer. The publisher is shown as **Ömer Kamil Örücü** (code-signed).
3. On first start, read and accept the **MerQur Pro license agreement**, then enter your **license key**.

To update, install the new version over the existing one; your license, settings and templates are kept.
**Help → Check for updates** tells you when a new version is available.

---

## 🔑 License

MerQur Pro is **paid software** and runs only with a **personal license key**:

- The key is issued to a named person and is valid for **one year**. The holder's name and institution appear in the About window and in report footers.
- Without a valid key the program does not open. The free [MerQur](https://github.com/omerorucu/merqur) remains available at no cost.
- **Commercial use is permitted** under the license.
- Licenses are sold and invoiced by **Sekizgen Academy**, the authorised reseller.

📧 **To obtain a license:** [info@sekizgenacademy.com](mailto:info@sekizgenacademy.com) · 🌐 [sekizgenacademy.com](https://sekizgenacademy.com)

Full terms: [EULA-PRO-EN.md](EULA-PRO-EN.md) · [EULA-PRO-TR.md](EULA-PRO-TR.md)

**Third-party software:** MerQur Pro includes MrBayes 3.2.9 (GNU GPL v3) as a separate program; its license
and unmodified source code are in the installation folder (`pro\ucuncu_taraf\mrbayes`). R packages are not
distributed with MerQur Pro.

The MerQur Pro source code is not public. This repository is for distribution only (installer, license
text, release notes).

---

## 📖 Citation

> Örücü, Ö. K. (2026). *MerQur Pro: Integrated Academic Data Analysis and Reporting Platform* (Version 3.5.0; base version 2.5.0) [Computer software]. https://doi.org/10.53463/merqur.2026001

Please also cite the R packages and programs listed in the "Software and citations" section of your results.

Registered work: T.C. Ministry of Culture and Tourism, registration no. **2026/18517**.

---

<details>
<summary><b>🇹🇷 Türkçe</b></summary>

## MerQur Pro nedir?

**MerQur Pro**, [MerQur](https://github.com/omerorucu/merqur)'un lisanslı sürümüdür. **MerQur 2.5.0'ın
tamamını** (143 form tabanlı analiz, 7 harita yöntemi, APA 7 raporları) içerir; buna **212 doğrulanmış
analiz şablonu** ve formla ifade edilemeyen analizler için bir **Kod sekmesi** ekler.

**Pro'nun getirdikleri**

- **212 doğrulanmış şablon, 24 kategori:** her şablon yayımlanmış bir kaynakla, eşdeğer yordam varsa SAS ile karşılaştırıldı. Öne çıkanlar:
  - ekonometri: ARDL/NARDL, kırılmalı birim kök, ikinci kuşak panel, SFA, DEA, kesikli seçim;
  - klinik: klinik tahmin modeli, cezalı Cox, RMST, çapraz geçiş, biyoeşdeğerlik;
  - orman ağacı ıslahı ve nicel genetik: orijin–döl denemesi, kalıtım derecesi ve genetik korelasyon, seleksiyon indeksleri, QST–FST, tohum bahçesinde çeşitlilik, klon ve çok lokasyonlu denemeler;
  - genetik ve filocoğrafya: dizi verisiyle AMOVA, MrBayes ile Bayesçi filogeni, DNA barkodlama, hizalama;
  - ekoloji: çevresel gradyan boyunca topluluk ağırlıklı ortalamalar (özellik CWM, satır/sütun/max permütasyon testleri), PERMANOVA ve yayılım (PERMDISP), doluluk modelleri;
  - diğer: oran meta-analizi, RI-CLPM, dialel, karışım deneyleri, uzay-zaman krigingi.
- **Parametre ayarları penceresi:** yöntemin anlamlı bütün seçenekleri Değişkenler, Model, Seçenekler, Gelişmiş ve Çıktı sekmelerinde ayarlanabilir. Toplam 2.935 parametre var. **Tamam ve çalıştır** analizi bu ayarlarla çalıştırır.
- **MrBayes 3.2.9 birlikte gelir:** Bayesçi filogeni ek kurulum gerektirmez.
- **Yazılım ve atıflar:** her koşuda MerQur Pro, R/Python ve kullanılan paketler sürümleri ve resmî atıflarıyla listelenir; makalenin yöntem bölümüne doğrudan yapıştırılabilir. `.mqs` betiği farklı paket sürümleriyle yeniden çalıştırılırsa uyarı verilir.
- **Kod sekmesi:** gömülü Python 3.13, bilgisayardaki R 4.5.x; `mq` modülüyle MerQur motorları koddan çağrılır.
- **AI Yorumlayıcı:** kendi API anahtarınızla sonuç ve rapor yorumu. Veri hücreleri gönderilmez; yapay zekâ sonuçları hesaplamaz ya da değiştirmez.
- Ücretsiz MerQur ile **yan yana** kurulur.

**Sistem gereksinimleri:** Windows 10/11 64 bit, yaklaşık 1,5 GB disk. R şablonları (212'nin 185'i) için R 4.5.x gerekir. Program yalnız sizin gönderdiğiniz AI isteklerinde ve **Yardım → Güncellemeleri Denetle** ile ağa çıkar.

**Kurulum ve güncelleme:** [Son sürümden](https://github.com/omerorucu/merqur_pro/releases/latest) `MerQurPro-3.5.0-windows-x64-Setup.exe` indirilir ve çalıştırılır. Yeni sürüm mevcut kurulumun üzerine kurulur; lisans, ayarlar ve şablonlar korunur.

**Lisans:** MerQur Pro ücretlidir ve kişiye özel, **bir yıllık** lisans anahtarıyla çalışır. **Ticari kullanım serbesttir.** Satış ve faturalama yetkili satıcı **Sekizgen Academy** tarafından yapılır.
Lisans için: [info@sekizgenacademy.com](mailto:info@sekizgenacademy.com) · [sekizgenacademy.com](https://sekizgenacademy.com) · Sözleşme: [EULA-PRO-TR.md](EULA-PRO-TR.md)

**Üçüncü taraf yazılım:** MrBayes 3.2.9 (GNU GPL v3) ayrı bir program olarak birlikte gelir; lisans metni ve değiştirilmemiş kaynak kodu kurulum klasöründedir.

**Atıf:** Örücü, Ö. K. (2026). *MerQur Pro: Bütünleşik Akademik Veri Analizi ve Raporlama Platformu* (Sürüm 3.5.0; temel sürüm 2.5.0) [Bilgisayar yazılımı]. https://doi.org/10.53463/merqur.2026001 — Sonuçlardaki "Yazılım ve atıflar" bölümünde listelenen paketlere de atıf yapılması rica olunur.

</details>

---

<div align="center">
<sub>© 2026 Ömer K. Örücü · All rights reserved · Eser Sicil No 2026/18517</sub>
</div>
