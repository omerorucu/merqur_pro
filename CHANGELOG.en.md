# MerQur Pro: Changelog

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
