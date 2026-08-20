SWMM5 / SWMM6 Web Tools - Gist Index
A collection of browser-based tools for exploring, QA/QC-ing, and visualizing EPA SWMM5 and SWMM6 models. Each runs entirely client-side - drop your .inp, .rpt, and .out files (or load from GitHub) and go. Built by Robert Dickinson.

Table of Contents
SWMM5 Theory & Numerics
QA/QC & Diagnostics
Engine & Solver Comparison
Hydrology & LID/Infiltration
Cross-Platform & Interop Guides
GIS & Data Workflows
History, People & Culture
Off-Topic / Side Projects
SWMM5 Theory & Numerics
The governing equations, convergence math, and solver theory underneath SWMM5/SWMM6 — for readers who want the "why," not just the "how."

OpenSWMM Engine Explorer
A searchable grid of 120 SWMM engine algorithms mapped to their governing equations (LaTeX), symbols, solver options, and source files, spanning numerics, hydrology/hydraulics, quality/LID, control/IO, plus 20 alpha SWMM6/OpenSWMM features.

App: https://open-swmm-engine-explorer.netlify.app
Gist: https://gist.github.com/dickinsonre/31826f736810b12f01ac71861719d621
The SWMM Refinement Manifold
A schematic infographic proposing a 6-axis convergence policy (Δt, Courant factor, lengthening tolerance, head/flow tolerances, minimum surface area) for benchmarking SWMM5 against SWMM6 on the same network.

App: https://swmm-refinement-manifold.netlify.app
Gist: https://gist.github.com/dickinsonre/10804cdfddb44f58d93c1e0c6a0ef4e3
ReSWMM CFL Analyzer
Courant–Friedrichs–Lewy stability analysis for ICM SWMM networks, with .inp file parsing, a stability map, three discretization methods (Fixed, CFL-based, AASD), sourced to Roesner et al. (1988) and Pachaly et al. (2019).

App: https://auburn-reswmm.netlify.app
Gist: https://gist.github.com/dickinsonre/9bd36dc44992179db05b0b4f84f9388b
SWMM5 Lengthening Advisor
Interactive tool explaining what LENGTHENING_STEP really does in SWMM5's dynamic wave routing, source-validated against EPA SWMM 5.2.4 (link.c) — network advisor, Pareto trade-off sweep, and improvement roadmap.

App: https://swmm5-conduit-lengthening-advisor.netlify.app
Gist: https://gist.github.com/dickinsonre/7f23e206ce8a238e2bd086e08c12a915
Anderson Acceleration for SWMM6 - Interactive Explainer
An interactive companion to Caleb Buahin's proposal for speeding up the SWMM6 dynamic wave solver with depth-2 Anderson Acceleration. Method credit: Caleb Buahin (EPA ORD / Hazen and Sawyer).

App: https://swmm6-anderson-acceleration.netlify.app
Gist: https://gist.github.com/dickinsonre/9937e7ba673607b47f5492837b34ed7f
OpenSWMM Caleb Anderson Acceleration
Convergence animator, iteration-count histograms, and a per-node skip-list evaluator for stability fallbacks — companion to Buahin's Anderson Acceleration proposal for the OpenSWMM (SWMM6) dynamic-wave solver.

App: https://openswmm-caleb-anderson-acceleration.netlify.app
Gist: https://gist.github.com/dickinsonre/82e25f1210fed459b669f9f6f5274e2d
RDII Reimagined — SWMM2D Process-Based Initial Abstraction
Interactive companion to Caleb Buahin's proposal replacing SWMM's linear monthly-R RDII surrogate with an exponential, temperature-driven soil-moisture reservoir — year simulator, single-storm convolution, recovery curves, and a climate stress test.

App: https://rdii-reimagined-swmm2d.netlify.app
Gist: https://gist.github.com/dickinsonre/f3fb45c1c7bb2f84270831e5aa191251
Equifinality Explorer — SWMM Subcatchment GLUE
Interactive GLUE calibration simulator on a verified nonlinear-reservoir SWMM subcatchment model — Latin Hypercube sampling, NSE/KGE behavioral thresholds, dotty plots, weighted parameter uncertainty, and a lumped-reservoir vs. kinematic-wave numerical-scheme comparison.

App: https://equafinality-swmm-explorer.netlify.app
Gist: https://gist.github.com/dickinsonre/a4ca2ab2d53143b2cea157623abff2c5
Double Pendulum Wave → SWMM5
Interactive chaos-to-hydraulics tool tracing a classic double pendulum wave's sensitive-dependence trajectories into real SWMM5 sewer geometry — illustrating equifinality, invert-profile stress testing, and DYNWAVE Courant stability through live physics.

App: https://double-pendulum-swmm5.netlify.app
Gist: https://gist.github.com/dickinsonre/47729405548fbf00b7775d9d10f6eb39
SOM Explorer — Self-Organizing Maps for SWMM Calibration
Interactive Kohonen SOM trained on Monte Carlo calibration of a verified mini SWMM-style runoff engine — equifinality made visible via mean-NSE, U-Matrix, hits, and component-plane map views, plus a live SOM-folding playground and full 13-check verification receipt.

App: https://swmm-som-explorer.netlify.app
Gist: https://gist.github.com/dickinsonre/dd8fea8eef6bad6154944dcbd31858e9
QA/QC & Diagnostics
Tools for validating a finished run, spotting numerical trouble, and visualizing results in 3D.

SWMM5 .OUT Singular-Value Spectrum
In-browser SVD analyzer for EPA SWMM binary .out results — reveals how many independent temporal-spatial patterns a model's results actually contain (A = UΣVᵗ), with exact and randomized methods, rank-k compression readout, and engine-verified findings showing real SWMM output is strongly low-rank.

App: https://swmm5-swmm6-svs.netlify.app
Gist: https://gist.github.com/dickinsonre/614175dd0556648785436f93319d9ef7
SWMM5 Model Map: Plan & Orbit Explorer
Dual-view .inp visualizer pairing a true-coordinate GIS plan view with a novel torus "orbit" layout (flow order = angle, elevation = tube height) — critical-path tracing, 5 color-by modes, GitHub repo browsing, and CSV/SVG/GIF export.

App: https://swmm5-orbit-map.netlify.app
Gist: https://gist.github.com/dickinsonre/8fc757c9d4d2dfdc89cc736bb79fe656
SWMM5 & SWMM6 Phase Space Explorer
Cross-plots flow against depth to reveal the loop rating curve - the hydraulic analog of a phase-space orbit. Includes a model-wide sweep that ranks every element by loop geometry, oscillation, surcharge, and backwater signatures, cross-checked against the .rpt engine diagnostics.

App: https://swmm5-swmm6-phase-space.netlify.app
Gist: https://gist.github.com/dickinsonre/5657a4b8af03cf76842fd35a08e952ae
SWMM5 Inspector Rover
A robot that QA/QCs your SWMM5 model and narrates the output — load your .inp, .rpt, and .out files and let the Rover walk your network, flag problems, and answer questions about what happened during the run.

App: https://swmm5-out-inspector-rover.netlify.app
Gist: https://gist.github.com/dickinsonre/9619008f7603e534cc663be48810d71e
SWMM5 Emergence Lab
An in-browser lab for studying emergence in stormwater networks, testing whether a drainage network behaves as more than the sum of its parts. Every experiment is checked against 118 real SWMM 5.2 simulations used as ground truth.

App: https://swmm-emergence-lab.netlify.app
Gist: https://gist.github.com/dickinsonre/965d619e303aee892150cd6442036c32
SWMM5 Benchmark 3D Viewer
An OWA SWMM5 Test Suite viewer that loads .inp/.rpt/.out files and renders the EXTRAN Manual benchmark networks in true 3D, complete with animated results playback.

App: https://swmm5-3d-viewer.netlify.app
Gist: https://gist.github.com/dickinsonre/2ff8c0e29b4aed084601ee9e4a13fe38
SWMM5 Network State-Space Morph
D3-based network visualizer that animates a real combined-sewer SWMM5 model morphing between geographic, elevation-profile, and topological-hierarchy layouts, with downstream BFS tracing and reachability diagnostics.

App: https://nathan-mel-state-space-swmm5.netlify.app
Gist: https://gist.github.com/dickinsonre/e81df83a548a3741808d6b7a3d34b66c
Log-Scaled Hilbert Curve → SWMM5 Network Generator
Builds a single serial SWMM5 conduit chain following a Hilbert curve's traversal order with logarithmically scaled lengths spanning orders of magnitude, purpose-built to stress-test the dynamic wave solver — with an in-browser WASM SWMM engine, adaptive bisection loop, batch experiment export, and a .rpt benchmark reader.

App: https://log-scaled-hilbert-swmm5-inp-file.netlify.app
Gist: https://gist.github.com/dickinsonre/92c38c4f24a4b6ab566d4c9e2bc31df3
Engine & Solver Comparison
Head-to-head comparisons of SWMM5, SWMM6/OpenSWMM, and competing commercial engines.

Two SWMM Engines in the Browser — LocalSWMM SWMM5/SWMM6 Deep-Dive
Runs genuine SWMM5 (EPA 5.2.2) and SWMM6 (OpenSWMM v6.0.0-alpha.2) WebAssembly engines side by side, prompted by Joaquín Alvarado's LocalSWMM (Chile) — testing run isolation, state surface, hot-start carryover, and numerical divergence, with three findings including an Anderson-acceleration fix.

App: https://localswmm-swmm5-swmm6-engine-chile.netlify.app
Gist: https://gist.github.com/dickinsonre/ccbdd004c1c667c2e9fbae1167fbb66d
SWMM5 Nesterov Optimizer Racer
Races plain gradient descent against Nesterov's Accelerated Gradient (1983) as they calibrate a genuine EPA SWMM 5.2 WebAssembly engine live in-browser, spending real engine runs as currency — with a loss-surface heatmap, live descent paths, and honest caveats about non-convexity.

App: https://swmm5-nestorov-optimizer.netlify.app
Gist: https://gist.github.com/dickinsonre/8b5c6300120efc1fa2933b5c3ae920e0
SWMM5 Engine Harness
Interactive lab running the real EPA SWMM 5.2.2 WebAssembly engine live in-browser — tweak routing step, lengthening step, max trials, head tolerance, and variable-step factor, and watch continuity error, a flow-depth phase portrait, and a full parameter sensitivity sweep respond.

App: https://swmm5-engine-harness.netlify.app
Gist: https://gist.github.com/dickinsonre/8bc28c44b4fecfd1f88fab668c5857b0
SWMM Moonshine Round-Trip Verifier — SWMM5 ⇄ SWMM6
Compares two EPA SWMM binary .out result sets element-by-element and issues a machine-checked certificate (tolerance bands, continuity gate, SHA-256 hashes) proving two engine runs matched — styled after @introsp3ctor's monstrous-moonshine visualizer.

App: https://swmm-moonshine-engine-scenario-compar.netlify.app
Gist: https://gist.github.com/dickinsonre/2c6d54433826ea2a8024784430d8b0ea
Four-Engine Pipe Comparator
Solver-numerics lab, feature matrix, and terminology rosetta comparing HEC-RAS Pipe Networks 7.0, InfoWorks ICM, EPA SWMM5, and the SWMM6 track (SWMM5+/OpenSWMM), with 5 shared benchmark systems and a hydrograph-comparison tool.

App: https://four-engine-comparison.netlify.app
Gist: https://gist.github.com/dickinsonre/cd250efdcb80c178278de1924d7ee86e
XPSWMM TUFLOW Louise
Triple-checked reference on what's changed in the TUFLOW engine (Classic → GPU → HPC) since FEMA's 2011 acceptance of XPSWMM 2D, with release timeline, solver comparison, and FEMA status breakdown.

App: https://xpswmm-tuflow-louise.netlify.app
Gist: https://gist.github.com/dickinsonre/6f0bbc3ee72a05e7eee962614863b847
Hydrology & LID/Infiltration
Tools focused on runoff generation, infiltration, LID/BMP performance, and test-case building.

Dragon Fold Watersheds (SWMM5 Runoff Code Interactive)
Fractal-derived SWMM5 subcatchment & LID studio — carves watersheds from a Heighway dragon curve, runs a real embedded SWMM5 WebAssembly engine for before/after LID comparisons.

App: https://dragon-swmm5-runoff-code-interactive.netlify.app
Gist: https://gist.github.com/dickinsonre/e234b5f21fcd53d9f49d419fb8ad8bce
Meadow Creek & Pond - A Watershed You Can Walk Into
An interactive 3D watershed with rolling hills, a meandering creek, and a pond with a spillway notch, all reacting live to simulated rainfall, infiltration, and runoff. One click exports the terrain as a runnable EPA SWMM5 model.

App: https://meadow-creek-pond-swmm5-swmm6.netlify.app
Gist: https://gist.github.com/dickinsonre/695c05ed4684ada120f75059fb213e6b
SWMM5 and SWMM6 Rosette Subcatchment Generator
A single-file, browser-based tool that procedurally generates radially-symmetric ("rosette") subcatchment networks, useful as reproducible test cases or teaching examples.

App: https://swmm5-swmm6-rosette-inp.netlify.app
Gist: https://gist.github.com/dickinsonre/f801c5302a7c21b21de9a155c7745436
The Bowl Is Full - Soil Compaction and the Apparent Curve Number
An interactive SWMM5 Horton infiltration model showing how a compacted subsoil layer creates a "bowl-limited" runoff response exceeding TR-55 curve number predictions. Concept credit: Dr. Shirley Clark, Penn State Harrisburg.

App: https://bowl-full-horton-cn-swmm5-sclark.netlify.app
Gist: https://gist.github.com/dickinsonre/6f6b1118df9f49c81c1451011d9e35b5
Bioretention Infiltration, Over Time
Interactive reading of a 4-year, 24-mesocosm field study (Skorobogatov et al. 2026) showing bioretention infiltration rising rather than clogging, mapped onto SWMM5 Bio-Retention Cell, ICM SuDS, and SWMM6 LID parameters.

App: https://bioretention-infiltration-swmm-kwl.netlify.app
Gist: https://gist.github.com/dickinsonre/6f3681e28a86d5f1a4c3c391094a380c
Building a SWMM5 Model for PySWMM LID Studies
Getting-started guide for building a SWMM5 .inp file from raw DEM, pipe, and land-use data entirely via Python — covers .inp structure, swmm-api build scripts, PySWMM validation, LID_CONTROLS/LID_USAGE setup.

App: https://building-a-swmm5-no-ux-pyswmm.netlify.app
Gist: https://gist.github.com/dickinsonre/b7bbd9fff5d7954fccf5bb85d64d1b3d
Cross-Platform & Interop Guides
Guides translating between SWMM5 and other commercial/open platforms.

ICMT Explorer — InfoWorks ICM Transportable Database Reader
Fully client-side reader for InfoWorks ICM's .icmt Transportable Database format — decodes the reverse-engineered object tree and replays nested SWMM network commit logs into tables, a map, and a runnable SWMM5 .inp export, verified by a 50-test Node harness.

App: https://icmt-explorer-for-swmm.netlify.app
Gist: https://gist.github.com/dickinsonre/8f3aca942b79555ce65a172909e033b1
SWMM5 ↔ ICM Comparison Model Selector — 30 Benchmark Archetypes
Interactive catalog of 30 benchmark models for isolating specific SWMM5-vs-ICM InfoWorks engine behaviors across hydrology, conveyance, structures, controls, water quality, and numerics — with value/effort ranking, a sortable matrix, and a recommended run order.

App: https://swmm5-icm-comparison-test-files.netlify.app
Gist: https://gist.github.com/dickinsonre/be970d28e4b29fd2f24bc40b675d65aa
EPANET Total Head Explorer
Hands-on companion to EPANET's total-head math — from Elevation + Pressure = Total Head through a series-network Hazen-Williams headloss walk to a step-by-step hand solve of the Global Gradient Algorithm (Todini & Pilati, 1988) on a looped network.

App: https://epanet-total-head-explorer.netlify.app
Gist: https://gist.github.com/dickinsonre/f19288456d5d1d55eeceae6f2c42832a
ICM Ruby Script Picker
Browsable, searchable catalog of InfoWorks ICM Ruby scripts with live parameter fields that rewrite the source code, one-click copy/download, CSV export, and a bring-your-own-catalog scripts.json loader.

App: https://icm-ruby-picker.netlify.app
Gist: https://gist.github.com/dickinsonre/479ea7fba865e50c2eb8cda245e59e45
InfoSWMM Explained
An interactive teardown of the ArcMap-era Innovyze InfoSWMM platform — how it combined the EPA SWMM5 engine, ArcMap-based GIS integration, DBF-based attribute storage, and ArcGIS feature geometry, plus legacy model recovery workflows.

App: https://infoswmm-explained.netlify.app
Gist: https://gist.github.com/dickinsonre/18e1648d1cb06009707cb468b42593ce
InfoDrainage in 30 Minutes - for SWMM5 Experts
A fast-start translation guide for SWMM5 users learning Autodesk InfoDrainage — auto-design, the 15+ BMP SuDS library, ~8 hydrology methods (FEH/FSR, TR-55, Rational), the embedded SWMM5 engine, Civil 3D interop, and a SWMM5-to-IDDX converter.

App: https://infodrainage-30min.netlify.app
Gist: https://gist.github.com/dickinsonre/40c6c0c52c0c7240723e18e07e2114ea
ICM SewerGEMS Comparison
Interactive step-by-step guide for taking a SewerGEMS stormwater network into InfoWorks ICM as a 1D pipe model and coupling it to a 2D surface flood mesh, with a live rainfall/surcharge demo and decision guide.

App: https://icm-sewergems-comparison.netlify.app
Gist: https://gist.github.com/dickinsonre/45de5555fdd5028b6db49b1388e28b5e
PRV Modeling for Better Pressure Management
Interactive engineering guide contrasting simplified PRV set-point control against physical valve response — live opening-percentage workbench, EPANET/InfoWater Pro/WS Pro capability comparison, and four design-review scenarios.

App: https://ng-prv-blog-wspro-explainer.netlify.app
Gist: https://gist.github.com/dickinsonre/e087273b625066dca849a37cfcd5fdb7
Rural Water Analysis Explainer — KYPipe PDD Curves
Interactive explainer of KYPipe's Peak Demand Diversity curve method for rural water system design — live PDD calculator, branch-line sizing example, and an EPANET/WaterGEMS comparison.

App: https://rural-kypipe-starter.netlify.app
Gist: https://gist.github.com/dickinsonre/4103511df30781016c907b5382273768
One Backbone — SWMM · EPANET · WNTR on One SQL Layer
An explorable test of Raza Ali's proposal for a unified SWMM/EPANET/WNTR data layer, built on a real in-browser SQLite database with engine-validated exports and four statistical tests for cross-system leak detection.

App: https://one-water-backbone-sewntr.netlify.app
Gist: https://gist.github.com/dickinsonre/7f71e63d029174a6039d15527a83aa6d
Medearis Workflow Explorer
Interactive deconstruction of Tim Medearis's Ruby + AI + Exchange automation pipeline for InfoWorks ICM/WS Pro — parameterized AI prompt builder, Ruby/Exchange code examples, and a dashboard mockup.

App: https://medearis-ruby-workflow.netlify.app
Gist: https://gist.github.com/dickinsonre/3b4e6564b74aa66a5a6b51d718ff435e
GIS & Data Workflows
Tools for pulling in real-world GIS data and browsing code repositories.

Naperville GIS & ESRI Data Explorer
Browsable catalog of every public ArcGIS REST endpoint the City of Naperville exposes (11 service folders, 21 EnerGov layers) — copy-ready query URLs plus SWMM, InfoWorks ICM (ODIC/Ruby Exchange), and EPANET (Python/epyt) import workflows.

App: https://naperville-gis-swmm-icm-epanet-data.netlify.app
Gist: https://gist.github.com/dickinsonre/d1286ad4f51528c37504dd4f6022495e
AWI Innovyze GitHub Viewer
Searchable file-tree browser for Autodesk Water Infrastructure's Open-Source-Support repo (1,903 files, 455 folders) — inline preview, product-based filtering across ICM/InfoWorks tools, and CSV/Markdown export.

App: https://awi-innovyze-github-viewer.netlify.app
Gist: https://gist.github.com/dickinsonre/9f2f53295ee0b3550a035065c0d3f4bf
Dickinson Code Wiki
AI-powered GitHub repo browser spanning the dickinsonre, SWMMBobSWMM6, CIMM-ORG, and SWMMEnablement accounts — file tree explorer, auto-generated Mermaid architecture diagrams, and a Claude-powered repo chat.

App: https://dickinsonre-repo-wiki.netlify.app
Gist: https://gist.github.com/dickinsonre/67076315d4858d94268f6a6da3499fc6
Unveiling Groundwater Potential in Hangu District, Pakistan
Interactive explainer of an open-access MDPI Water paper — GIS-driven Weight of Evidence and Frequency Ratio bivariate models ranking ten landscape factors, with a live site-scoring builder and ROC validation charts.

App: https://water-mdpi-hangu-district.netlify.app
Gist: https://gist.github.com/dickinsonre/bf36b0aa4087693f7cef4183761d03e5
XPSWMM .xp Card Reader → SWMM5 Converter
Browser-based parser for XPSWMM's 80-column punch-card .xp database format (rooted in 1981 SWMM Version 3), converting nodes, links, and job control to EPA SWMM 5 .inp — with single-file, local-folder-ZIP, and GitHub-folder batch conversion, validated against 38 real-world models.

App: https://xp-to-swmm5.netlify.app
Gist: https://gist.github.com/dickinsonre/f66f32b51c73f4ae6822b2d9ecbf2c51
ICM SQL Cookbook — Full Code with Comments
Searchable, filterable library of 95 fully-commented InfoWorks ICM and SWMM SQL scripts spanning spatial, simulation results, time series, 2D/mesh, connected objects, arrays, traversal, and QA/QC — with a query-starter skeleton generator and a tracked corrections log.

App: https://icm-sql-cookbook.netlify.app
Gist: https://gist.github.com/dickinsonre/4d3dd0a80f67ddc62f7feae6ed93e929
History, People & Culture
Tributes, retrospectives, and reflections on the SWMM community and its people.

Samer's ICM Explorer
Tribute and explainer app for Samer Muhandes' #DidYouKnowICMcandothat InfoWorks ICM video series — episode library, a featured infographic, and a breakdown of his four ICM network families.

App: https://samer-knows-icm-infoworks.netlify.app
Gist: https://gist.github.com/dickinsonre/5b9d75c0e16869ca378c84a0ee16e1b0
Visual SWMM 1999 CHI Conference
Interactive recreation of the circa-2000 Toronto CHI conference paper by Kuch, Dickinson, Akman, and Keskar on merging SWMM with a full civil engineering design package (Visual Hydro/CAiCE), with then/now barrier analysis and a SWMM5 theory update.

App: https://visual-swmm-1999-chi-conference.netlify.app
Gist: https://gist.github.com/dickinsonre/e714ef575fb97cbb9f0bb6b89655a450
Comprehension Debt Explorer
Interactive model of parallel fan-out vs. review capacity, showing how unreviewed work compounds into technical debt with interest, paired with a durability framework for what SWMM5/SWMM6 must preserve vs. disposable churn.

App: https://ky-time-management-idea.netlify.app
Gist: https://gist.github.com/dickinsonre/037243bf42bd6a20b99efc7d1ff6ad26
SWMM 6 Luck Surface Area
Interactive strategy builder applying the Luck Surface Area (Doing × Telling) framework to eleven ranked channels for supporting EPA SWMM 6 — live sliders, radar diagram, and a support-probability estimator.

App: https://my-swmm-luck-surface-area.netlify.app
Gist: https://gist.github.com/dickinsonre/0f4a835c7dc5f6a254185b8aa2f0bd67
Bob Dickinson's Three-Channel Repurposer
Content engine turning one idea into a canonical swmm5.org article, newsletter edition, LinkedIn post, and X thread/Article — with live SEO self-competition warnings and a publishing-order guide.

App: https://bob-dickinson-seo-guide.netlify.app
Gist: https://gist.github.com/dickinsonre/91323a5b0e6a8055a640d1bb1e11305c
SWMM5 Fourier Cross-Section Fitter
Fits any closed conduit boundary as a Fourier series in log r(θ) and emits a pasteable SWMM5 [CURVES] Shape block, validated directly against SWMM5's own built-in width tables — with live conveyance/area/width error metrics and a Henderson binary-expansion mode for smooth/spiky/fractal boundaries.

App: https://fourier-xsection-swmm5-swmm6.netlify.app
Gist: https://gist.github.com/dickinsonre/5b87c14d2d24255c97b7fc4e21feafed
Off-Topic / Side Projects
Tangential, non-stormwater explorations kept for fun and cross-pollination of ideas.

Pangea Rainfall Explorer
Interactive explainer of the Carnian Pluvial Episode, the Late Triassic "megamonsoon" wet phase caused by Wrangellia volcanism — volcanic-forcing simulator and paleo-terrain data source guide.

App: https://pangea-rainfall-explorer.netlify.app
Gist: https://gist.github.com/dickinsonre/59b011dd81e7edf43923def4e61d5457
Valles Marineris Water Models
Speculative settlement-engineering explorer for Mars's Valles Marineris canyon — habitat, atmosphere, and cost calculators alongside a real Hardy-Cross EPANET water network solver and a genuine SWMM5 nonlinear-reservoir stormwater model.

App: https://valles-marineris-water-models.netlify.app
Gist: https://gist.github.com/dickinsonre/65de2b49cf7b20e05de8d62ea41b05dc
The Macroscope — Howard T. Odum & the Energy Systems Language
Interactive field guide to Howard T. Odum's Energy Systems Language — biography and timeline, an 11-symbol energy circuit gallery, and a drag-and-drop diagram builder with SVG/GIF export.

App: https://ht-odum-energy-map.netlify.app
Gist: https://gist.github.com/dickinsonre/0e3c4353dc4376da0d4893cfadfce32c
Forest City, Johor — Interactive 3D Map
Stylised Three.js relief map of the Forest City reclaimed-island development in Johor, Malaysia — day/night toggle, satellite overlay, photo pinning, and clickable landmarks.

App: https://3d-forest-city-malaysia.netlify.app
Gist: https://gist.github.com/dickinsonre/1a4b348a64249509294bc12b5716237a
EPANET-Agentic
Interactive explainer of a multi-agent LLM system for natural-language control of EPANET simulations (Wang, Fu & Savic 2026), mapped onto SWMM5 and compared against Agentic SWMM (Zhang & Valeo 2026), the first peer-reviewed agentic SWMM workflow.

App: https://agentic-swmm-epanet-paper-reviews.netlify.app
Gist: https://gist.github.com/dickinsonre/b32c7b225d2c6959253e6f12f241f40e
Particle Life — Emergent Lifeforms
Recreation of Mathelirium's particle-life simulation — a drag-editable attraction/repulsion rule matrix between colored species produces crawling, hunting "creatures" with no programmed behavior, plus 14 presets, an evolving-rules mode, and GIF/PNG/JSON export.

App: https://particle-life-for-k.netlify.app
Gist: https://gist.github.com/dickinsonre/988907d4b750ca0167d492650f3e8abc
SWMM Aesop Fable Forge
AI fable generator casting weirs, orifices, pumps, and detention ponds as Aesop-style characters at true Aesop lengths (Brief/Classic/Extended), in English or Chinese, each hydraulically accurate with a moral for life and for modeling — 13-fable gallery works with no API.

App: https://swmm-aesop-fables.netlify.app
Gist: https://gist.github.com/dickinsonre/bf6ec6b96ecedeb60902c86d37256fd3
SWMM5 Documentation & Strategy Scorecard
Personal dashboard scoring three long-running goals — SWMM5 documentation coverage vs. ICM/HEC-RAS/SWMM6, ensuring SWMM6 surpasses SWMM5, and readying an alternate SWMM for 2030 — against real swmm5.org archive and GitHub repo data, with status badges and next actions.

App: https://swmm-2030-strategy.netlify.app
Gist: https://gist.github.com/dickinsonre/2523aee89c24c0bb1c217917bce27e49
Last updated: August 2, 2026

More tools added over time. See all gists at https://gist.github.com/dickinsonre
