# Repository Structure

**Last Updated:** November 16, 2025

This document explains the organization of the `computational-emergence-theory` repository and the rationale behind each component.

---

## 📁 Current Structure (Phase 1)

```
computational-emergence-theory/
├── README.md                          # Main entry point (you are here!)
├── STRUCTURE.md                       # This document
├── CONTRIBUTING.md                    # Contribution guidelines
├── LICENSE                            # MIT License
│
├── papers/
│   ├── Paper1_Substrate_Architecture_Framework.md
│   │                                  # Level 0-3: Components → Agents (~8,500 words)
│   ├── Paper2_Multi_Scale_Emergence.md
│   │                                  # Level 3-6: Agents → Societies (~10,500 words)
│   ├── Paper3_Consciousness_Correlates.md
│   │                                  # Cross-cutting: Consciousness metrics (~14,000 words)
│   ├── abstracts/
│   │   ├── paper1_abstract.md         # Standalone abstracts
│   │   ├── paper2_abstract.md
│   │   └── paper3_abstract.md
│   └── supplementary/
│       ├── mathematical_derivations.md  # Formal proofs for emergence operators
│       ├── coarse_graining_examples.md  # Detailed examples of Φ functions
│       └── extended_predictions.md      # Additional testable hypotheses
│
├── theory/                            # Mathematical formalizations
│   ├── substrate_properties.py        # Φ_S vector characterization (from CS foundation)
│   ├── emergence_operators.py         # Coarse-graining functions Φ: L_i → L_{i+1}
│   ├── consciousness_metrics.py       # Six-dimensional measurement tools
│   ├── information_measures.py        # Integrated information (φ), transfer entropy
│   └── agent_models.py                # Perception-action-learning formalisms
│
├── implementations/                   # Simulation and analysis tools
│   ├── agent_modeling/
│   │   ├── perception_action_loop.py  # Level 3: Individual agent simulations
│   │   ├── learning_mechanisms.py     # Hebbian, gradient descent, reinforcement
│   │   └── README.md
│   ├── dyad_coordination/
│   │   ├── communication_models.py    # Level 4: Two-agent interactions
│   │   ├── theory_of_mind.py          # Modeling other's mental states
│   │   └── README.md
│   ├── collective_intelligence/
│   │   ├── group_dynamics.py          # Level 5: 3-150 agents
│   │   ├── information_aggregation.py # Wisdom of crowds, voting mechanisms
│   │   ├── network_effects.py         # Small-world, scale-free topology effects
│   │   └── README.md
│   ├── population_dynamics/
│   │   ├── phase_transitions.py       # Level 6: Social tipping points
│   │   ├── spreading_activation.py    # Diffusion models
│   │   ├── mean_field_approximation.py
│   │   └── README.md
│   └── hybrid_systems/
│       ├── human_ai_collaboration.py  # Mixed biological-artificial agents
│       ├── interface_models.py        # Bridging different substrates
│       └── README.md
│
├── data/                              # Empirical validation datasets
│   ├── biological/
│   │   ├── neural_recordings/         # fMRI, EEG for consciousness metrics
│   │   ├── behavioral_data/           # Human cognitive task performance
│   │   └── README.md
│   ├── artificial/
│   │   ├── ml_architectures/          # Transformer, RNN activation patterns
│   │   ├── agent_simulations/         # Multi-agent system outputs
│   │   └── README.md
│   └── hybrid/
│       ├── human_ai_interaction/      # Collaborative task data
│       ├── social_networks/           # Online community dynamics
│       └── README.md
│
├── predictions/                       # Testable hypotheses
│   ├── README.md                      # Overview of all predictions
│   ├── 01_substrate_agency/
│   │   ├── protocol.md                # How substrate shapes agent capabilities
│   │   ├── rationale.md
│   │   └── code/
│   ├── 02_dyad_bandwidth/
│   │   ├── protocol.md                # Communication bandwidth effects
│   │   ├── rationale.md
│   │   └── code/
│   ├── 03_group_size_performance/
│   │   ├── protocol.md                # Optimal group sizes for tasks
│   │   ├── rationale.md
│   │   └── code/
│   ├── 04_collective_intelligence/
│   │   ├── protocol.md                # Predicting c factor from composition
│   │   ├── rationale.md
│   │   └── code/
│   ├── 05_phase_transition_thresholds/
│   │   ├── protocol.md                # Social tipping point detection
│   │   ├── rationale.md
│   │   └── code/
│   ├── 06_hybrid_system_superiority/
│   │   ├── protocol.md                # Human-AI vs pure systems
│   │   ├── rationale.md
│   │   └── code/
│   └── 07_consciousness_architecture/
│       ├── protocol.md                # φ correlates with network properties
│       ├── rationale.md
│       └── code/
│
├── experiments/                       # Empirical validation
│   ├── README.md                      # Overview of experimental work
│   └── (experiments added as conducted)
│
├── notebooks/                         # Tutorials and demonstrations
│   ├── 01_emergence_operators.ipynb   # How to use coarse-graining functions
│   ├── 02_agent_modeling.ipynb        # Simulating Level 3 agents
│   ├── 03_collective_intelligence.ipynb  # Level 5 group dynamics
│   ├── 04_consciousness_metrics.ipynb # Measuring six dimensions
│   └── README.md
│
├── docs/                              # Accessible documentation
│   ├── glossary.md                    # Technical terms explained
│   ├── FAQs.md                        # Common questions
│   ├── key_insights.md                # Non-technical summary
│   ├── multi_scale_overview.md        # Visual guide to all levels
│   ├── consciousness_guide.md         # Understanding functional correlates
│   ├── practical_applications.md      # For practitioners (AI design, policy)
│   └── further_reading.md             # Related resources
│
├── figures/                           # Visual explanations
│   ├── conceptual/
│   │   ├── multi_scale_hierarchy.svg  # Levels 0-6 overview
│   │   ├── emergence_operators.svg    # Coarse-graining visualization
│   │   ├── agent_architecture.svg     # Perception-action-learning loop
│   │   ├── collective_intelligence.svg # Group dynamics patterns
│   │   └── consciousness_dimensions.svg # Six-dimensional space
│   ├── data/
│   │   └── (empirical results as they become available)
│   └── README.md                      # Figure descriptions and sources
│
├── references/
│   ├── bibliography.bib               # All 220+ citations across three papers
│   ├── key_papers/
│   │   ├── README.md                  # Annotated reading list
│   │   ├── substrate_foundations.md   # CS repo papers
│   │   ├── emergence_theory.md        # Complex systems, information theory
│   │   ├── collective_intelligence.md # Woolley, Malone, Surowiecki
│   │   ├── consciousness_theories.md  # IIT, GWT, HOT
│   │   └── multi_agent_systems.md     # Wooldridge, Russell & Norvig
│   └── tools.md                       # Software/hardware for testing
│
└── assets/
    ├── citation.bib                   # BibTeX for citing this work
    └── logos/                         # Branding (if needed)
```

---

## 🎯 Design Principles

### 1. **Modular Paper Structure**

Unlike the companion [computational-substrates](https://github.com/HillaryDanan/computational-substrates) repository (one comprehensive ~40k word paper), CET uses **three focused papers**:

- **Paper 1 (Foundation):** Reviews substrate-architecture (Levels 0-2), extends to agents (Level 3)
- **Paper 2 (Core Contribution):** Multi-scale emergence from agents to societies (Levels 3-6)
- **Paper 3 (Cross-cutting):** Consciousness correlates across all levels

**Rationale:** 
- Each paper can be published independently
- Different audiences (architects vs social scientists vs consciousness researchers)
- Clear progression: foundation → emergence → consciousness

### 2. **Separation of Theory and Implementation**

**Theory** (stable, mathematical):
- `papers/` - Formal frameworks
- `theory/` - Mathematical formalizations
- `docs/` - Conceptual explanations

**Implementation** (evolving, practical):
- `implementations/` - Simulation tools
- `notebooks/` - Tutorials
- `experiments/` - Empirical validation

### 3. **Level-Based Organization**

Implementations organized by organizational level:
- `agent_modeling/` - Level 3
- `dyad_coordination/` - Level 4
- `collective_intelligence/` - Level 5
- `population_dynamics/` - Level 6
- `hybrid_systems/` - Cross-level

**Principle:** Structure mirrors theoretical framework (Levels 0-6).

### 4. **Reproducibility First**

Following CS repo standards:
- Detailed protocols for all predictions
- Analysis code with dependencies listed
- Raw data (when shareable)
- Statistical methods documented
- Confidence intervals provided

**If someone can't reproduce it, we haven't communicated well enough.**

---

## 📈 Evolution Plan

### Phase 1: Foundation (Current - December 2025)

**Goal:** Establish three-paper framework and make it accessible.

**Deliverables:**
- ✅ Three core papers (Paper 1, 2, 3)
- ✅ README with clear positioning
- ⏳ Conceptual figures (multi-scale hierarchy, emergence operators)
- ⏳ Basic implementation tools (emergence operators, agent models)
- ⏳ Accessible documentation

**Files to create:**
```
figures/conceptual/*.svg        (5 key diagrams)
theory/*.py                     (5 core modules)
implementations/agent_modeling/ (basic agent simulations)
docs/*.md                       (6 accessibility documents)
```

### Phase 2: Implementation Development (January 2026)

**Goal:** Build tools for testing predictions across all levels.

**Deliverables:**
- Agent modeling framework (Level 3)
- Collective intelligence simulations (Level 5)
- Consciousness measurement tools (all levels)
- Jupyter notebook tutorials

**Files to create:**
```
implementations/agent_modeling/
    ├── perception_action_loop.py
    ├── learning_mechanisms.py
    ├── memory_systems.py
    └── README.md

implementations/collective_intelligence/
    ├── group_dynamics.py
    ├── information_aggregation.py
    ├── network_effects.py
    └── README.md

notebooks/
    ├── 01_emergence_operators.ipynb
    ├── 02_agent_modeling.ipynb
    ├── 03_collective_intelligence.ipynb
    └── 04_consciousness_metrics.ipynb
```

### Phase 3: Empirical Validation (Q1-Q2 2026)

**Goal:** Test predictions empirically across multiple levels.

**Priority experiments:**
1. **Agent-level:** Substrate-agency relationship (Prediction 1)
2. **Group-level:** Collective intelligence composition (Prediction 4)
3. **Population-level:** Phase transition thresholds (Prediction 5)

**Files to create:**
```
experiments/agent_substrate_matching/
    ├── README.md
    ├── methodology.md
    ├── data/
    ├── analysis/
    └── results.md

experiments/collective_intelligence_factors/
    ├── README.md
    ├── human_experiments/
    ├── simulation_validation/
    └── results.md

experiments/social_phase_transitions/
    ├── README.md
    ├── network_data/
    ├── tipping_point_detection/
    └── results.md
```

### Phase 4: Integration and Applications (Q3-Q4 2026)

**Goal:** Demonstrate practical applications and refine framework.

**Possible additions:**
```
applications/
    ├── human_ai_team_design/
    │   ├── composition_optimizer.py
    │   ├── task_allocation.py
    │   └── README.md
    ├── collective_intelligence_platforms/
    │   ├── design_principles.md
    │   ├── implementation_guide.md
    │   └── case_studies/
    └── emergent_capability_prediction/
        ├── scaling_law_analysis.py
        ├── capability_forecasting.py
        └── README.md

collaborations/
    ├── neuroscience_labs/          # Consciousness measurement validation
    ├── social_science_groups/      # Collective intelligence studies
    └── ai_safety_orgs/             # Emergent capability prediction
```

---

## 🗂️ File Naming Conventions

### General Rules
- Use `snake_case` for filenames: `emergence_operators.py`
- Use descriptive names: `phase_transition_detection.py` not `analysis2.py`
- Number papers: `Paper1_`, `Paper2_`, `Paper3_` (for clarity)
- Number notebooks sequentially: `01_emergence_operators.ipynb`
- Date experimental results: `results_2026_03_15.csv`

### Special Files
- `README.md` - Overview/index for each directory
- `protocol.md` - Experimental protocol (in predictions/)
- `rationale.md` - Motivation and importance (in predictions/)
- `results.md` - Findings from experiments

### Code
- Python modules: `descriptive_name.py` (snake_case)
- Classes: `CamelCase` (e.g., `EmergenceOperator`, `AgentModel`)
- Jupyter notebooks: `##_descriptive_name.ipynb` (numbered for sequence)
- Always include `requirements.txt` or `environment.yml`

---

## 🤝 Contributing to Structure

### Adding New Content

**New level-specific implementation?**
1. Determine level: 3 (agent), 4 (dyad), 5 (group), 6 (population)
2. Add to appropriate `implementations/` folder
3. Include tests and documentation
4. Update folder `README.md`

**New prediction?**
1. Create folder: `predictions/08_new_prediction/`
2. Add: `protocol.md`, `rationale.md`, `code/`, `README.md`
3. Update `predictions/README.md` to list it
4. Specify which level(s) it tests

**New experiment?**
1. Create folder: `experiments/experiment_name/`
2. Add: `README.md`, `methodology.md`, `data/`, `analysis/`, `results.md`
3. Update `experiments/README.md`
4. Link to relevant prediction(s)

**New figure?**
1. Add to `figures/conceptual/` or `figures/data/`
2. Use SVG for conceptual (scalable, editable)
3. Update `figures/README.md` with description
4. Reference in relevant paper(s)

**New documentation?**
1. Add to `docs/`
2. Link from main `README.md` if relevant
3. Keep accessible (avoid jargon, explain technical terms)
4. Provide examples

### Modifying Existing Content

**Paper updates:**
- **Minor fixes** (typos, clarifications): Edit paper directly
- **Major revisions** (new sections, reframing): Consider versioning
- Document changes in commit message
- Update abstract if substantive changes

**Code updates:**
- Follow semantic versioning (v0.1.0 → v0.2.0 for new features)
- Update docstrings and comments
- Add tests for new functionality
- Update `README.md` with new capabilities

**Experimental results:**
- **Never delete raw data** (archive if outdated)
- Add new analyses as separate files
- Document any corrections in `README.md`
- Maintain data provenance

---

## 📊 Size Guidelines

### Keep Files Manageable

**Papers:**
- Paper 1: ~8,500 words (foundation + Level 3)
- Paper 2: ~10,500 words (Levels 3-6, core contribution)
- Paper 3: ~14,000 words (consciousness, comprehensive)

**Code modules:**
- Single module: < 500 lines (split if larger)
- Well-documented with docstrings
- Clear separation of concerns

**Notebooks:**
- Tutorial notebooks: 20-50 cells (digestible in one sitting)
- Analysis notebooks: Can be longer but well-sectioned
- Always include markdown explanations

**Documentation:**
- Short docs: < 2,000 words (quick reference)
- Medium docs: 2,000-5,000 words (detailed guides)
- Link to papers for comprehensive treatment

### Data Files
- Raw data: CSV or HDF5 (open formats)
- Large files (>10MB): Consider external hosting (Zenodo, OSF, Figshare)
- Always include data dictionary
- Document collection methodology

---

## 🔍 Finding Things

### By Level of Analysis

**Want to understand Level 3 (Individual Agents)?**
→ `papers/Paper1_Substrate_Architecture_Framework.md` (Section 2)
→ `implementations/agent_modeling/`
→ `notebooks/02_agent_modeling.ipynb`

**Want to understand Levels 4-5 (Groups)?**
→ `papers/Paper2_Multi_Scale_Emergence.md` (Sections 3-4)
→ `implementations/collective_intelligence/`
→ `notebooks/03_collective_intelligence.ipynb`

**Want to understand Level 6 (Populations)?**
→ `papers/Paper2_Multi_Scale_Emergence.md` (Section 5)
→ `implementations/population_dynamics/`

**Want to understand consciousness across levels?**
→ `papers/Paper3_Consciousness_Correlates.md`
→ `theory/consciousness_metrics.py`
→ `notebooks/04_consciousness_metrics.ipynb`

### By Task

**I want to understand the framework:**
→ Start with `README.md`
→ Then `docs/multi_scale_overview.md`
→ Then read papers sequentially (1 → 2 → 3)

**I want to test a prediction:**
→ Go to `predictions/`
→ Pick prediction folder
→ Read `protocol.md` and `rationale.md`
→ Use code in `code/` folder

**I want to simulate agents/groups:**
→ Go to `implementations/`
→ Choose level-appropriate folder
→ Read folder `README.md`
→ Run example code or notebooks

**I want to cite this work:**
→ See `assets/citation.bib`
→ Or citation format in main `README.md`

**I need accessible explanation:**
→ Start with `docs/glossary.md`
→ Then `docs/key_insights.md`
→ Then `docs/multi_scale_overview.md`

### Search Tips

**GitHub search within this repo:**
```
repo:HillaryDanan/computational-emergence-theory [query]
```

**Search by level:**
```
"Level 3" OR "agent" OR "perception"      # Agent-level content
"Level 5" OR "group" OR "collective"      # Group-level content
"Level 6" OR "population" OR "phase"      # Population-level content
```

**Search by topic:**
```
language:Python emergence_operator        # Python code for operators
is:issue "collective intelligence"        # Issues discussing topic
```

---

## 📝 Maintenance

### Regular Updates
- Update `STRUCTURE.md` when adding major new sections
- Update `README.md` roadmap quarterly
- Update `predictions/README.md` as predictions are tested
- Keep `references/bibliography.bib` current with new citations
- Update paper cross-references if one paper changes substantially

### Version Control
- **Papers:** Major updates warrant version tags (v1.0, v1.1)
  - Paper 1 v1.0 → v1.1 if substantial addition to Level 3
  - Document changes in commit message
- **Code:** Semantic versioning (v0.1.0, v0.2.0, v1.0.0)
  - v0.x.y = pre-release (API may change)
  - v1.x.y = stable (backward compatible)
- **Protocols:** Version if changed (`protocol_v2.md`)

### Deprecation
- Move deprecated content to `archive/` folder
- Mark deprecated files: `**⚠️ DEPRECATED - See [new location]**`
- Never delete—maintain for reproducibility
- Document why deprecated and what replaces it

---

## 🎯 Design Philosophy

**1. Multi-Scale Integration**
- Structure mirrors theoretical levels (0-6)
- Cross-references between levels explicit
- Emergence operators connect levels formally

**2. Modular Papers**
- Each paper can stand alone
- Together they form coherent framework
- Clear progression: foundation → emergence → consciousness

**3. Theory-Implementation Linkage**
- Mathematical formalisms (`theory/`) correspond to simulations (`implementations/`)
- Papers provide theory, code provides tools
- Notebooks bridge theory and implementation

**4. Accessibility Gradient**
- General audience: `docs/` → `README.md`
- Practitioners: `implementations/` → `notebooks/`
- Researchers: `papers/` → `theory/`
- Everyone can find appropriate entry point

**5. Reproducibility and Openness**
- All code open source (MIT license)
- All data (when shareable) publicly available
- All methods fully documented
- Invite collaboration and replication

---

## 🔗 Relationship to Computational Substrates Repository

This repository **extends** the foundation established in [computational-substrates](https://github.com/HillaryDanan/computational-substrates):

**computational-substrates provides:**
- Substrate property formalization (Φ_S vector)
- Thermodynamic constraints (Landauer, von Neumann bottleneck)
- Architecture-substrate mapping (Levels 0-2)
- Substrate-appropriate algorithm design

**CET imports these foundations and extends:**
- From architectures (Level 2) to agents (Level 3)
- From agents to societies (Levels 4-6)
- Formalizes emergence via coarse-graining operators
- Applies to collective intelligence and social dynamics

**Together:** Complete multi-scale framework from transistors/neurons to civilizations.

**Cross-repo navigation:**
- CET Paper 1 Section 1 reviews CS foundations
- CET theory/ uses substrate_properties.py from CS concepts
- Both repos share information-theoretic grounding
- Both maintain same scientific rigor standards

---

## 🚀 Future Considerations

As this repository grows, we may add:

**Community Features:**
- `discussions/` - For questions, ideas, debates
- `contributors.md` - Acknowledge contributors
- `changelog.md` - Track significant changes

**Educational Content:**
- `tutorials/` - Step-by-step learning paths
- `lectures/` - Slide decks or recorded presentations
- `workshops/` - Hands-on exercises by level

**Applications:**
- `tools/` - Python packages for emergence analysis
- `demos/` - Interactive web demonstrations
- `case_studies/` - Real-world applications

**Collaboration:**
- `collaborations/` - Joint work with other labs
- `replications/` - Others testing our predictions
- `extensions/` - Novel applications of framework

**We'll add these as needed—not prematurely.**

---

## ❓ Questions?

If this structure is unclear or you're not sure where something belongs:

1. Check if similar content already exists (use GitHub search)
2. Ask in [Discussions](../../discussions) or [Issues](../../issues)
3. Consider which level (0-6) the content addresses
4. Propose structure changes (PRs welcome!)
5. When in doubt, document your reasoning in a README.md

**Principle:** If you're confused about where something goes, others will be too. Better to ask than to guess.

---

## 📊 Structure Health Metrics

We'll track (informally):
- **Discoverability:** Can people find content by level or topic?
- **Completeness:** Are all levels adequately documented/implemented?
- **Consistency:** Do we follow level-based organization principles?
- **Accessibility:** Can non-experts navigate successfully?
- **Integration:** Are cross-level connections clear?

**Feedback welcome!** This structure serves the content—if it's not working, we'll change it.

---

**Structure designed for:** Multi-scale integration, modular papers, theory-implementation linkage, and reproducibility.

**Structure evolves with:** New empirical findings, community contributions, and applications.

**Structure serves:** The core mission of understanding emergence from agents to societies with rigorous, testable, and impactful science.

---

*Last updated: November 16, 2025*  
*See git history for structure evolution*  
*Companion to: [computational-substrates](https://github.com/HillaryDanan/computational-substrates)*
