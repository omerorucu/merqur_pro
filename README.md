<div align="center">

<img src="icon/MerQurPro_icon_256.png" alt="MerQur Pro" width="160" />

# MerQur Pro

### *Analysis beyond the form: code, templates and the MerQur engine in one place*

**ANALYZE · MODEL · INTERPRET · REPORT**

*İNCELE · MODELLE · YORUMLA · RAPORLA*

**Integrated Academic Data Analysis & Reporting Platform: licensed edition**
*by Ömer K. Örücü*

---

![Version](https://img.shields.io/badge/version-3.0.0-5B21B6?style=flat-square)
![Base](https://img.shields.io/badge/base%20MerQur-2.3.1-7C3AED?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue?style=flat-square)
![Languages](https://img.shields.io/badge/i18n-TR%20%7C%20EN%20%7C%20ES-success?style=flat-square)
![Templates](https://img.shields.io/badge/code%20templates-165%20in%2023%20categories-5B21B6?style=flat-square)
![License](https://img.shields.io/badge/license-commercial%20key%20required-orange?style=flat-square)

**[⬇ Download MerQur Pro 3.0.0 for Windows](https://github.com/omerorucu/merqur_pro/releases/latest)**

</div>

---

## 🔍 What is MerQur Pro?

**MerQur Pro** is the licensed edition of [MerQur](https://github.com/omerorucu/merqur). It contains
**everything in MerQur 2.3.1** (137 form-based analyses, 7 map methods, APA 7 reports) and adds a
**Code tab** for analyses that a form cannot express: custom models, simulations, special contrasts
and methods MerQur does not offer as a form.

Code results do not live in a separate console. Every table, figure and text block your code produces
becomes a card in MerQur's **Results, Table, Chart and Report** tabs, goes into the DOCX report with its
code, and is saved with the project.

<div align="center">

| **165** | **23** | **2** | **APA 7** |
|:---:|:---:|:---:|:---:|
| Ready-to-run<br>code templates | Template<br>categories | Languages<br>(Python · R) | Reports with<br>code appendix |

</div>

MerQur Pro installs **side by side** with the free MerQur: separate folder, settings, recent files and
Start-menu icon. Installing or removing one does not affect the other.

---

## ✨ What Pro adds

### 🧑‍💻 Code tab: Python and R
- **Embedded Python 3.13** with numpy, scipy, pandas, statsmodels, scikit-learn and matplotlib. Nothing to install.
- **R** (4.5.x) through your own R installation, detected automatically. Missing packages come with a ready `install.packages(...)` suggestion.
- **Your own Python**, if you need packages beyond the embedded set (shown as "external" in the output footer).
- The active dataset is available as **`df`** in both languages. Turkish and Unicode column and level names are preserved.
- Safe execution: runs in a separate worker process, **Cancel stops it within a second**, with a configurable time limit. A crash in your code never takes the main window down.
- Syntax errors are highlighted on the offending line. A run history lets you reopen any earlier code.

### 📚 Template library: 165 ready analyses
Each template opens with a **parameter form** built from its definition, ships with **sample data and
sample parameters**, and its output is fully translated (TR / EN / ES: text, tables, comments).
Templates were checked against the source R/Python package and published worked examples. Where an
equivalent SAS procedure exists, its code is shown next to the template for comparison.

| Category | # | Examples |
|---|:---:|---|
| Genetics & genomics | 23 | kinship, AMOVA, GWAS, genomic selection, QTL mapping, heritability, qPCR relative quantification |
| Causal inference | 16 | double machine learning, AIPW, TMLE, synthetic control, staggered DiD, regression discontinuity |
| Mixed models | 12 | ordinal mixed (CLMM), multi-response mixed, advanced GLMM, glmmTMB families |
| Regression models | 11 | beta regression, hurdle, exact logistic, panel Tobit, custom likelihood |
| Time series | 11 | ARFIMA, wavelets, DCC-GARCH, general state space |
| Multivariate | 10 | Bayesian networks, compositional data, functional data |
| Psychometrics | 10 | network psychometrics, cognitive diagnosis, many-facet Rasch, advanced DIF |
| Survival | 10 | interval-censored regression, multi-state models, flexible parametric |
| Structural equation models | 8 | Bayesian SEM, growth mixture, multilevel CFA, ESEM |
| Meta-analysis | 7 | network meta, multivariate meta, multilevel meta, dose–response meta |
| Spatial | 7 | areal Bayesian CAR, conditional simulation, MGWR, point process models |
| Design of experiments | 5 | alpha lattice, group sequential, fractional factorial, optimal design |
| Quality | 5 | CUSUM / EWMA, process capability, reliability, control and attribute charts |
| Resampling | 5 | block bootstrap, custom bootstrap, delta method |
| Survey | 4 | calibration / raking, small-area estimation, sample selection, hot-deck |
| Smoothing | 4 | GAMLSS, GAMM, advanced quantile regression, MARS |
| Ecology | 4 | diversity indices, constrained ordination, PERMANOVA / Mantel |
| Bayesian | 3 | Bayesian model averaging, multilevel brms, custom MCMC models |
| Simulation | 3 | power by simulation, mixed-model power, method comparison simulation |
| Missing data | 2 | multilevel imputation, MNAR reference-based imputation |
| Extreme values | 2 | GEV / GPD |
| Method comparison | 1 | Deming and Passing–Bablok |
| Starters | 2 | empty Python and R templates |

Save your own code as a template ("Save as template…"); it appears in the same tree.

### ⚙️ MerQur engine from code
The `mq` module calls MerQur's own analysis engines from Python, for example `mq.ttest(df, "y", "g")` or
`mq.mediation(...)`, and returns exactly the text MerQur's form would produce. `mq.yardim("ttest")`
lists the options. `mq.veriye_yaz(...)` writes new columns or filtered rows back to the Data tab
**after a confirmation dialog**, and the change can be undone (Ctrl+Z).

### 🤖 AI assistant
- **AI code assistant** under the Code tab: describe an analysis in Turkish or English and get code, have an error explained with a corrected version shown as a diff, or have the output interpreted.
- **AI Interpreter** for results and reports.
- Uses **your own API key** for the provider you choose, stored in the Windows credential vault. Only column names and summaries are sent; **data cells are never sent**, and the preview window shows exactly what will go out.

### 📜 Scripts (.mqs) with code steps
MerQur scripts can contain code steps. In the GUI each code step asks for approval. In headless runs they
run only with `--kod-izin`, so a shared script cannot run code on your machine without your consent.

---

## 💻 System requirements

| | |
|---|---|
| **Operating system** | Windows 10 or 11, 64-bit |
| **Disk** | about 1.5 GB |
| **Memory** | 8 GB recommended |
| **R (optional)** | R 4.5.x, needed for the R templates (139 of 165). Packages are installed from within R when a template asks for them. |
| **Internet** | not required. MerQur Pro makes **no network requests** except AI requests you send yourself. |

macOS and Linux builds of MerQur Pro are not available yet. The free MerQur runs on all three.

---

## 📥 Installation

1. Download **`MerQurPro-3.0.0-windows-x64-Setup.exe`** from the [latest release](https://github.com/omerorucu/merqur_pro/releases/latest).
2. Run the installer. The publisher is shown as **Ömer Kamil Örücü** (code-signed).
3. On first start, read and accept the **MerQur Pro license agreement**, then enter your **license key**.

The language, theme, font size, chart DPI and AI provider settings of an existing free MerQur are
copied once on first start.

---

## 🔑 License

MerQur Pro is **paid software** and runs only with a **personal license key**:

- The key is issued to a named person and is valid for **one year**. The holder's name and institution appear in the About window and in report footers.
- Without a valid key the program does not open. The free [MerQur](https://github.com/omerorucu/merqur) remains available at no cost.
- **Commercial use is permitted** under the license.
- Licenses are sold and invoiced by **Sekizgen Academy**, the authorised reseller.

📧 **To obtain a license:** [info@sekizgenacademy.com](mailto:info@sekizgenacademy.com) · 🌐 [sekizgenacademy.com](https://sekizgenacademy.com)

Full terms: [EULA-PRO-EN.md](EULA-PRO-EN.md) · [EULA-PRO-TR.md](EULA-PRO-TR.md)

The source code is not public. This repository is for distribution only (installer, license text,
release notes).

---

## 📖 Citation

> Örücü, Ö. K. (2026). *MerQur Pro: Integrated Academic Data Analysis and Reporting Platform* (Version 3.0.0; base version 2.3.1) [Computer software]. https://doi.org/10.53463/merqur.2026001

Registered work: T.C. Ministry of Culture and Tourism, registration no. **2026/18517**.

---

<details>
<summary><b>🇹🇷 Türkçe</b></summary>

## MerQur Pro nedir?

**MerQur Pro**, [MerQur](https://github.com/omerorucu/merqur)'un lisanslı sürümüdür. **MerQur 2.3.1'in
tamamını** (137 form tabanlı analiz, 7 harita yöntemi, APA 7 raporları) içerir ve formla ifade
edilemeyen analizler için bir **Kod sekmesi** ekler: özel modeller, benzetimler, özel kontrastlar ve
MerQur'da form olarak bulunmayan yöntemler.

Kodun ürettiği her tablo, grafik ve metin MerQur'un **Sonuçlar, Tablo, Grafik ve Rapor** sekmelerine kart
olarak düşer, koduyla birlikte DOCX raporuna girer ve projeyle kaydedilir.

**Pro'nun getirdikleri**

- **Kod sekmesi:** gömülü Python 3.13 (numpy, scipy, pandas, statsmodels, scikit-learn, matplotlib); bilgisayardaki R 4.5.x; isteğe bağlı kendi Python'unuz. Etkin veri iki dilde de `df`. Ayrı işçi süreçte güvenli çalışma, 1 saniyede iptal, zaman sınırı, hata satırı vurgusu, geçmiş.
- **165 hazır şablon, 23 kategori:** genetik (23), nedensel çıkarım (16), karma modeller (12), regresyon modelleri (11), zaman serisi (11), çok değişkenli (10), psikometri (10), sağkalım (10), YEM (8), meta-analiz (7), uzamsal (7) ve diğerleri. Her şablonun parametre formu, örnek verisi ve örnek parametreleri vardır; çıktıları TR/EN/ES çevrilidir.
- **Koddan MerQur motoru:** `mq.ttest(...)`, `mq.mediation(...)` formla aynı sonucu verir. `mq.veriye_yaz(...)` onay penceresiyle Veri sekmesine yazar ve geri alınabilir.
- **Yapay zekâ yardımcısı:** Türkçe istekten kod, hata açıklama (fark görünümüyle düzeltme), çıktı yorumu ve AI Yorumlayıcı. Kendi API anahtarınızla çalışır. Veri hücreleri gönderilmez, yalnız sütun adları ve özetler gider.
- **Kod adımlı .mqs betikleri:** arayüzde adım başına onay, başsız çalıştırmada yalnız `--kod-izin` ile.
- Ücretsiz MerQur ile **yan yana** kurulur. Klasörler, ayarlar ve kısayollar ayrıdır.

**Sistem gereksinimleri:** Windows 10/11 64 bit, yaklaşık 1,5 GB disk. R şablonları (165'in 139'u) için R 4.5.x gerekir. İnternet gerekmez. Program, sizin gönderdiğiniz AI istekleri dışında ağa çıkmaz.

**Kurulum:** [Son sürümden](https://github.com/omerorucu/merqur_pro/releases/latest) `MerQurPro-3.0.0-windows-x64-Setup.exe` indirilir ve çalıştırılır. İlk açılışta lisans sözleşmesi kabul edilir ve lisans anahtarı girilir.

**Lisans:** MerQur Pro ücretlidir ve kişiye özel, **bir yıllık** lisans anahtarıyla çalışır. **Ticari kullanım serbesttir.** Satış ve faturalama yetkili satıcı **Sekizgen Academy** tarafından yapılır.
Lisans için: [info@sekizgenacademy.com](mailto:info@sekizgenacademy.com) · [sekizgenacademy.com](https://sekizgenacademy.com) · Sözleşme: [EULA-PRO-TR.md](EULA-PRO-TR.md)

**Atıf:** Örücü, Ö. K. (2026). *MerQur Pro: Bütünleşik Akademik Veri Analizi ve Raporlama Platformu* (Sürüm 3.0.0; temel sürüm 2.3.1) [Bilgisayar yazılımı]. https://doi.org/10.53463/merqur.2026001

</details>

---

<div align="center">
<sub>© 2026 Ömer K. Örücü · All rights reserved · Eser Sicil No 2026/18517</sub>
</div>
