<div align="center">

# 🌊 SWMM5 / SWMM6 Web Tools — Gist Index 🌊

### A Collection of Browser-Based Tools for Exploring, QA/QC-ing & Visualizing EPA SWMM Models

![Client-Side](https://img.shields.io/badge/Runs-100%25%20Client--Side-00b4d8?style=for-the-badge&logo=javascript&logoColor=white)
![Built by](https://img.shields.io/badge/Built%20by-Robert%20Dickinson-8e44ad?style=for-the-badge)
![Gists](https://img.shields.io/badge/Gists-40%2B-f39c12?style=for-the-badge&logo=github)
![Last Updated](https://img.shields.io/badge/Updated-Aug%202%2C%202026-27ae60?style=for-the-badge)

Each tool runs entirely client-side — drop your `.inp`, `.rpt`, and `.out` files (or load from GitHub) and go. 🚀

</div>

---

## 📑 Table of Contents

| 🧮 [Theory & Numerics](#-swmm5-theory--numerics) | 🩺 [QA/QC & Diagnostics](#-qaqc--diagnostics) | ⚙️ [Engine Comparison](#️-engine--solver-comparison) |
|---|---|---|
| 🌧️ [Hydrology & LID](#️-hydrology--lidinfiltration) | 🔀 [Cross-Platform Guides](#-cross-platform--interop-guides) | 🗺️ [GIS & Data](#️-gis--data-workflows) |
| 📜 [History & Culture](#-history-people--culture) | 🎲 [Off-Topic / Side Projects](#-off-topic--side-projects) | |

---

## 🧮 SWMM5 Theory & Numerics
> *The governing equations, convergence math, and solver theory underneath SWMM5/SWMM6.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **OpenSWMM Engine Explorer** | 120 SWMM engine algorithms mapped to LaTeX equations, symbols, solver options & source files | [App](https://open-swmm-engine-explorer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/31826f736810b12f01ac71861719d621) |
| **SWMM Refinement Manifold** | 6-axis convergence policy benchmarking SWMM5 vs SWMM6 | [App](https://swmm-refinement-manifold.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/10804cdfddb44f58d93c1e0c6a0ef4e3) |
| **ReSWMM CFL Analyzer** | CFL stability analysis for ICM SWMM networks, 3 discretization methods | [App](https://auburn-reswmm.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/9bd36dc44992179db05b0b4f84f9388b) |
| **SWMM5 Lengthening Advisor** | Explains `LENGTHENING_STEP` in dynamic wave routing, source-validated | [App](https://swmm5-conduit-lengthening-advisor.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/7f23e206ce8a238e2bd086e08c12a915) |
| **Anderson Acceleration Explainer** | Companion to Caleb Buahin's depth-2 Anderson Acceleration proposal | [App](https://swmm6-anderson-acceleration.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/9937e7ba673607b47f5492837b34ed7f) |
| **OpenSWMM Caleb Anderson Acceleration** | Convergence animator & iteration-count histograms | [App](https://openswmm-caleb-anderson-acceleration.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/82e25f1210fed459b669f9f6f5274e2d) |
| **RDII Reimagined** | Process-based initial abstraction replacing linear monthly-R RDII | [App](https://rdii-reimagined-swmm2d.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/f3fb45c1c7bb2f84270831e5aa191251) |
| **Equifinality Explorer (GLUE)** | GLUE calibration, Latin Hypercube sampling, NSE/KGE thresholds | [App](https://equafinality-swmm-explorer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/a4ca2ab2d53143b2cea157623abff2c5) |
| **Double Pendulum Wave → SWMM5** | Chaos-to-hydraulics tool tracing pendulum trajectories into sewer geometry | [App](https://double-pendulum-swmm5.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/47729405548fbf00b7775d9d10f6eb39) |
| **SOM Explorer** | Self-Organizing Maps for SWMM calibration equifinality | [App](https://swmm-som-explorer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/dd8fea8eef6bad6154944dcbd31858e9) |

---

## 🩺 QA/QC & Diagnostics
> *Tools for validating a finished run, spotting numerical trouble, and 3D visualization.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **SWMM5 .OUT Singular-Value Spectrum** | SVD analyzer revealing rank of temporal-spatial patterns in `.out` results | [App](https://swmm5-swmm6-svs.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/614175dd0556648785436f93319d9ef7) |
| **Plan & Orbit Explorer** | Dual-view GIS plan + torus "orbit" layout with critical-path tracing | [App](https://swmm5-orbit-map.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/8fc757c9d4d2dfdc89cc736bb79fe656) |
| **Phase Space Explorer** | Flow-vs-depth loop rating curve analog to phase-space orbits | [App](https://swmm5-swmm6-phase-space.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/5657a4b8af03cf76842fd35a08e952ae) |
| **SWMM5 Inspector Rover** | Robot that QA/QCs your model and narrates the output | [App](https://swmm5-out-inspector-rover.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/9619008f7603e534cc663be48810d71e) |
| **SWMM5 Emergence Lab** | Tests emergent network behavior vs. 118 real SWMM 5.2 simulations | [App](https://swmm-emergence-lab.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/965d619e303aee892150cd6442036c32) |
| **SWMM5 Benchmark 3D Viewer** | EXTRAN Manual benchmark networks in true 3D w/ animated playback | [App](https://swmm5-3d-viewer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/2ff8c0e29b4aed084601ee9e4a13fe38) |
| **Network State-Space Morph** | D3 network morph between geographic/elevation/topological layouts | [App](https://nathan-mel-state-space-swmm5.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/e81df83a548a3741808d6b7a3d34b66c) |
| **Hilbert Curve Network Generator** | Log-scaled Hilbert-curve conduit chain stress-testing dynamic wave solver | [App](https://log-scaled-hilbert-swmm5-inp-file.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/92c38c4f24a4b6ab566d4c9e2bc31df3) |

---

## ⚙️ Engine & Solver Comparison
> *Head-to-head comparisons of SWMM5, SWMM6/OpenSWMM, and competing commercial engines.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **LocalSWMM Deep-Dive** | SWMM5 vs SWMM6 WASM engines side by side, run isolation & hot-start | [App](https://localswmm-swmm5-swmm6-engine-chile.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/ccbdd004c1c667c2e9fbae1167fbb66d) |
| **Nesterov Optimizer Racer** | Gradient descent vs. Nesterov Acceleration calibrating live SWMM engine | [App](https://swmm5-nestorov-optimizer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/8b5c6300120efc1fa2933b5c3ae920e0) |
| **SWMM5 Engine Harness** | Live WASM engine lab — routing step, tolerance, sensitivity sweep | [App](https://swmm5-engine-harness.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/8bc28c44b4fecfd1f88fab668c5857b0) |
| **Moonshine Round-Trip Verifier** | Machine-checked certificate proving SWMM5 ⇄ SWMM6 result matches | [App](https://swmm-moonshine-engine-scenario-compar.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/2c6d54433826ea2a8024784430d8b0ea) |
| **Four-Engine Pipe Comparator** | HEC-RAS 7.0, ICM, SWMM5, SWMM6 solver-numerics & terminology rosetta | [App](https://four-engine-comparison.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/cd250efdcb80c178278de1924d7ee86e) |
| **XPSWMM TUFLOW Louise** | TUFLOW engine changes since FEMA's 2011 XPSWMM 2D acceptance | [App](https://xpswmm-tuflow-louise.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/6f0bbc3ee72a05e7eee962614863b847) |

---

## 🌧️ Hydrology & LID/Infiltration
> *Runoff generation, infiltration, LID/BMP performance, and test-case building.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **Dragon Fold Watersheds** | Fractal Heighway-dragon-derived subcatchments + LID studio | [App](https://dragon-swmm5-runoff-code-interactive.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/e234b5f21fcd53d9f49d419fb8ad8bce) |
| **Meadow Creek & Pond** | 3D walkable watershed exporting to a runnable SWMM5 model | [App](https://meadow-creek-pond-swmm5-swmm6.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/695c05ed4684ada120f75059fb213e6b) |
| **Rosette Subcatchment Generator** | Procedural radially-symmetric test-case subcatchments | [App](https://swmm5-swmm6-rosette-inp.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/f801c5302a7c21b21de9a155c7745436) |
| **The Bowl Is Full** | Compacted-subsoil Horton infiltration vs. TR-55 curve numbers | [App](https://bowl-full-horton-cn-swmm5-sclark.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/6f6b1118df9f49c81c1451011d9e35b5) |
| **Bioretention Infiltration Over Time** | 4-year field study mapped onto SWMM5/ICM SuDS/SWMM6 LID params | [App](https://bioretention-infiltration-swmm-kwl.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/6f3681e28a86d5f1a4c3c391094a380c) |
| **PySWMM LID Studies Guide** | Build a `.inp` from DEM/pipe/land-use data via Python | [App](https://building-a-swmm5-no-ux-pyswmm.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/b7bbd9fff5d7954fccf5bb85d64d1b3d) |

---

## 🔀 Cross-Platform & Interop Guides
> *Guides translating between SWMM5 and other commercial/open platforms.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **ICMT Explorer** | Client-side reader for InfoWorks ICM's `.icmt` transportable DB format | [App](https://icmt-explorer-for-swmm.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/8f3aca942b79555ce65a172909e033b1) |
| **30 Benchmark Archetypes** | Catalog isolating SWMM5-vs-ICM engine behaviors | [App](https://swmm5-icm-comparison-test-files.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/be970d28e4b29fd2f24bc40b675d65aa) |
| **EPANET Total Head Explorer** | Elevation+Pressure=Total Head, Global Gradient Algorithm walk | [App](https://epanet-total-head-explorer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/f19288456d5d1d55eeceae6f2c42832a) |
| **ICM Ruby Script Picker** | Searchable ICM Ruby scripts w/ live parameter rewriting | [App](https://icm-ruby-picker.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/479ea7fba865e50c2eb8cda245e59e45) |
| **InfoSWMM Explained** | Teardown of ArcMap-era Innovyze InfoSWMM platform | [App](https://infoswmm-explained.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/18e1648d1cb06009707cb468b42593ce) |
| **InfoDrainage in 30 Minutes** | Fast-start guide for SWMM5 users learning Autodesk InfoDrainage | [App](https://infodrainage-30min.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/40c6c0c52c0c7240723e18e07e2114ea) |
| **ICM SewerGEMS Comparison** | SewerGEMS → ICM 1D/2D coupling guide | [App](https://icm-sewergems-comparison.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/45de5555fdd5028b6db49b1388e28b5e) |
| **PRV Modeling Guide** | Set-point vs. physical valve response, EPANET/InfoWater/WS Pro | [App](https://ng-prv-blog-wspro-explainer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/e087273b625066dca849a37cfcd5fdb7) |
| **KYPipe PDD Curves** | Peak Demand Diversity method for rural water design | [App](https://rural-kypipe-starter.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/4103511df30781016c907b5382273768) |
| **One Backbone (SWMM·EPANET·WNTR)** | Unified SQL data layer w/ cross-system leak detection | [App](https://one-water-backbone-sewntr.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/7f71e63d029174a6039d15527a83aa6d) |
| **Medearis Workflow Explorer** | Ruby + AI + Exchange automation pipeline for ICM/WS Pro | [App](https://medearis-ruby-workflow.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/3b4e6564b74aa66a5a6b51d718ff435e) |

---

## 🗺️ GIS & Data Workflows
> *Tools for pulling in real-world GIS data and browsing code repositories.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **Naperville GIS & ESRI Data Explorer** | 11 service folders, 21 EnerGov layers, ready-made query URLs | [App](https://naperville-gis-swmm-icm-epanet-data.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/d1286ad4f51528c37504dd4f6022495e) |
| **AWI Innovyze GitHub Viewer** | 1,903-file browser for Autodesk Water Infra's open-source repo | [App](https://awi-innovyze-github-viewer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/9f2f53295ee0b3550a035065c0d3f4bf) |
| **Dickinson Code Wiki** | AI-powered repo browser across 4 GitHub accounts w/ Claude chat | [App](https://dickinsonre-repo-wiki.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/67076315d4858d94268f6a6da3499fc6) |
| **Hangu District Groundwater** | GIS Weight-of-Evidence groundwater potential explainer | [App](https://water-mdpi-hangu-district.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/bf36b0aa4087693f7cef4183761d03e5) |
| **XPSWMM .xp Card Reader** | Converts 1981-era punch-card `.xp` format to SWMM5 `.inp` | [App](https://xp-to-swmm5.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/f66f32b51c73f4ae6822b2d9ecbf2c51) |
| **ICM SQL Cookbook** | 95 fully-commented ICM/SWMM SQL scripts | [App](https://icm-sql-cookbook.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/4d3dd0a80f67ddc62f7feae6ed93e929) |

---

## 📜 History, People & Culture
> *Tributes, retrospectives, and reflections on the SWMM community.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **Samer's ICM Explorer** | Tribute to Samer Muhandes' #DidYouKnowICMcandothat series | [App](https://samer-knows-icm-infoworks.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/5b9d75c0e16869ca378c84a0ee16e1b0) |
| **Visual SWMM 1999 CHI Conference** | Recreation of Kuch/Dickinson/Akman/Keskar's Visual Hydro/CAiCE paper | [App](https://visual-swmm-1999-chi-conference.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/e714ef575fb97cbb9f0bb6b89655a450) |
| **Comprehension Debt Explorer** | Fan-out vs review capacity, technical debt with interest | [App](https://ky-time-management-idea.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/037243bf42bd6a20b99efc7d1ff6ad26) |
| **SWMM6 Luck Surface Area** | Doing × Telling framework for supporting EPA SWMM6 | [App](https://my-swmm-luck-surface-area.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/0f4a835c7dc5f6a254185b8aa2f0bd67) |
| **Three-Channel Repurposer** | Turns one idea into blog/newsletter/LinkedIn/X content | [App](https://bob-dickinson-seo-guide.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/91323a5b0e6a8055a640d1bb1e11305c) |
| **Fourier Cross-Section Fitter** | Fits closed conduit boundaries as Fourier series → SWMM5 Shape block | [App](https://fourier-xsection-swmm5-swmm6.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/5b87c14d2d24255c97b7fc4e21feafed) |

---

## 🎲 Off-Topic / Side Projects
> *Tangential, non-stormwater explorations kept for fun and cross-pollination of ideas.*

| 🔧 Tool | 📝 Description | 🔗 Links |
|---|---|---|
| **Pangea Rainfall Explorer** | Carnian Pluvial Episode "megamonsoon" volcanic-forcing simulator | [App](https://pangea-rainfall-explorer.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/59b011dd81e7edf43923def4e61d5457) |
| **Valles Marineris Water Models** | Speculative Mars canyon settlement w/ Hardy-Cross EPANET solver | [App](https://valles-marineris-water-models.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/65de2b49cf7b20e05de8d62ea41b05dc) |
| **The Macroscope (H.T. Odum)** | Energy Systems Language gallery + diagram builder | [App](https://ht-odum-energy-map.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/0e3c4353dc4376da0d4893cfadfce32c) |
| **Forest City, Johor 3D Map** | Three.js relief map w/ day/night toggle & photo pinning | [App](https://3d-forest-city-malaysia.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/1a4b348a64249509294bc12b5716237a) |
| **EPANET-Agentic** | Multi-agent LLM control of EPANET, mapped to Agentic SWMM | [App](https://agentic-swmm-epanet-paper-reviews.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/b32c7b225d2c6959253e6f12f241f40e) |
| **Particle Life** | Emergent creature simulation via attraction/repulsion rules | [App](https://particle-life-for-k.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/988907d4b750ca0167d492650f3e8abc) |
| **SWMM Aesop Fable Forge** | AI fable generator casting weirs & pumps as Aesop characters | [App](https://swmm-aesop-fables.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/bf6ec6b96ecedeb60902c86d37256fd3) |
| **SWMM5 Strategy Scorecard** | Dashboard tracking documentation coverage & SWMM6 roadmap goals | [App](https://swmm-2030-strategy.netlify.app/) · [Gist](https://gist.github.com/dickinsonre/2523aee89c24c0bb1c217917bce27e49) |

---

<div align="center">

📅 **Last updated:** August 2, 2026 · 🔎 More tools added over time
See all gists → **[gist.github.com/dickinsonre](https://gist.github.com/dickinsonre)**

Made with 💧 by **[Robert Dickinson](https://github.com/dickinsonre)**

</div>
