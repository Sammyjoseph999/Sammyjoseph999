# Hi, I'm Sammy

I build data and machine learning tools, mostly in Python. My main work is on climate data for agriculture; alongside it I build LLM applications (retrieval, tool-using agents) and keep a set of analysis and modelling projects here.

## What I work on

- **Climate data tooling.** Core contributor to [climate-toolkit](https://github.com/CGIAR-Climate-Data-Hub/climate-toolkit), an open-source Python package from the CGIAR Climate Data Hub that gives one interface to eleven climate datasets (CHIRPS, AgERA5, ERA5, TAMSAT, NASA POWER, CMIP6 and others). It is on PyPI: `pip install climate-toolkit`.
- **LLM applications.** Retrieval-augmented question answering and tool-using agents, with the exact rules kept in tested code and the model used only for the fuzzy parts.
- **Applied machine learning.** Classification, regression and clustering on real datasets, with held-out evaluation and honest baselines.

## Selected projects

### Search and LLM applications

| Project | What it is | Result |
|---|---|---|
| [arxiv-hybrid-search](https://github.com/Sammyjoseph999/arxiv-hybrid-search) | Keyword, vector and hybrid search compared on 5,000 arXiv papers | Keywords win for a known paper (93% against 84%), vectors for a topic; rank-fusion hybrid was worse than keywords alone |
| [vibration-monitoring-rag](https://github.com/Sammyjoseph999/vibration-monitoring-rag) | RAG assistant over vendor and reference pages, running locally on open models | Right source ranked first for 10 of 10 test questions after a chunking fix |
| [car-manual-rag](https://github.com/Sammyjoseph999/car-manual-rag) | Dashboard-warning assistant that retrieves and quotes a car manual | Right entry first for 31 of 32 warnings, against 24 of 32 for fixed-size chunks |
| [bird-count-intake-agent](https://github.com/Sammyjoseph999/bird-count-intake-agent) | Tool-using agent (FastMCP + OpenAI) that cleans messy field notes into validated records | Rules enforced in a tool layer covered by 49 offline tests |

### Machine learning

| Project | What it is | Result |
|---|---|---|
| [used-car-prices](https://github.com/Sammyjoseph999/used-car-prices) | Price model on 427,000 Craigslist listings, with the cleaning tested | 44% of usable listings were reposts; removing them changes the test score from 13% to an honest 16% median error |
| [insurance-charges](https://github.com/Sammyjoseph999/insurance-charges) | What drives medical insurance charges, with three models compared | A linear model with one smoker/BMI interaction beats tuned gradient boosting (R² 0.91 against 0.90) |
| [ipo-listing-gains-pytorch](https://github.com/Sammyjoseph999/ipo-listing-gains-pytorch) | PyTorch classifier for IPO listing gains, compared with logistic regression | 65-67% accuracy over 20 splits against a 55% baseline; the simple model wins |

### Data analysis

| Project | What it is | Result |
|---|---|---|
| [student-evaluation-response-styles](https://github.com/Sammyjoseph999/student-evaluation-response-styles) | How 5,820 course evaluations were actually filled in | 51% of students gave one answer to all 28 questions, which reshuffles course rankings |
| [east-africa-economic-indicators](https://github.com/Sammyjoseph999/east-africa-economic-indicators) | Growth and structural change in six economies, from the World Bank API | Income per person tripled in Ethiopia and Rwanda since 2000 and did not change in Burundi |

More analysis and modelling projects are in my [repositories](https://github.com/Sammyjoseph999?tab=repositories).

## Tools I use

- **Languages:** Python, SQL
- **Data and modelling:** pandas, NumPy, scikit-learn, PyTorch, statsmodels, MLflow
- **LLM applications:** sentence-transformers, Hugging Face Transformers, LangChain, LlamaIndex, FastMCP, OpenAI API
- **Geospatial and climate:** xarray, Google Earth Engine
- **Practice:** pytest, Git, Jupyter, DuckDB

## How I work

Each project here states its data source, runs from a clean environment, and reports results against a baseline, including the ones that turned out modest.
