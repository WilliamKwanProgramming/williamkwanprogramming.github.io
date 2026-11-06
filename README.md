# Statistician – Quantitative Finance and Insurance-Linked Securities

#### Technical Skills

- **Quantitative:** Probability, Stochastic Processes, Monte Carlo, Time Series, Regression, Hypothesis Testing, Backtesting
- **Machine Learning:** Feature Engineering, Gradient Boosting, Clustering, Anomaly Detection, PyTorch, TensorFlow
- **Finance & Risk:** Fixed Income, Options Pricing, Portfolio Theory, Relative Value, VaR/TVaR, Stress Tests, Cat Bonds
- **Programming & Tools:** Python (NumPy, pandas), C++, R, SQL, Snowflake, Databricks, AWS, Excel, Bloomberg
- **Other:** Power BI, MATLAB, Adobe Suite (AutoCAD, Acrobat), Microsoft Office, LaTeX, Linux, Networking

## Education
- M.S., Statistics | University of Toronto (_June 2027_)
- B.S., Mathematics and Statistics | University of Toronto (_June 2025_)

## Quantitative Finance and Insurance-Linked Securities Projects

### Limit Order Book Simulator and Market-Making Backtester
[Repository](https://github.com/WilliamKwanProgramming/limit-order-book-market-maker)
A C++17 limit order book with Python bindings (pybind11) that handles more than 10 million simulated messages per second with 300 resting orders and 2.6 million per second with a million, a replayer for LOBSTER-format message files that checks the book against the recorded state after every message (0 mismatches on 3 million synthetic rows; not yet run on real LOBSTER data), and a market-making backtester. Over 2,000 paired simulated episodes, Avellaneda-Stoikov quoting reduces the standard deviation of P&L by 78% and of inventory by 61% compared with symmetric quoting, at USD 14.9 lower mean P&L per episode; a follow-up decomposition shows that the inventory skew alone gives the same reduction in P&L standard deviation. Under Hawkes bursts of informed order flow every strategy loses money, and Avellaneda-Stoikov loses USD 126 more per episode than symmetric quoting. Simulated data only; tests and continuous integration included.

### Cat Bond Issuance Model
[Repository](https://github.com/WilliamKwanProgramming/cat-bond-issuance-model)
Simulates 100,000 years of Florida hurricane losses (calibrated to HURDAT2) on a hypothetical USD 100 bn portfolio and structures three USD 500 million layers with expected losses of 3.90%, 1.98% and 1.09%, with uncertainty bands from 200 refits of the hazard model. A regression of log spread on log expected loss for 56 public cat bond layers with US named-storm exposure, specified before it was run, gives a slope of 0.466 with year effects (wild cluster bootstrap 95% interval 0.115 to 0.830); the pre-specified test of proportional pricing (slope 1) rejects only when eight flagged rows are included. Also includes an Excel layer pricer with live formulas, a 12-page pitchbook and a test suite (39 of 39 deliberately injected bugs caught).

### Market Risk Engine: VaR, Expected Shortfall and Backtesting
[Repository](https://github.com/WilliamKwanProgramming/market-risk-engine)
A Python library that forecasts one-day 99% value-at-risk and 97.5% expected shortfall with seven methods (historical simulation, EWMA, filtered historical simulation with a GARCH-t model, Monte Carlo), revalues option positions in full, and backtests the forecasts with coverage, independence, expected shortfall and scoring tests; a Streamlit dashboard shows the results. It was validated first on simulated data with known truth, then backtested under a protocol fixed beforehand on 7,300 days of prices of 20 US stocks and the S&P 500 index: Holm-adjusted Kupiec tests reject every method except filtered historical simulation, and EWMA with a normal distribution breached the 99% VaR on 2.14% of days. 151 tests, and a mutation check that catches 38 of 38 deliberately injected bugs.

### Landfall: Hurricane Event-Driven Trading Strategy
[Repository](https://github.com/WilliamKwanProgramming/landfall-hurricane-trading-strategy)
Tests whether the prices of hurricane-exposed US stocks react to National Hurricane Center information around landfalls. A Python and C++ pipeline detects landfalls in HURDAT2 data, forecasts tracks with a model refit each season on earlier seasons only (72-hour error 734 km against 957 km for persistence) and computes wind footprints (the C++ kernel runs 2.4 times faster than NumPy). A pre-specified event study of 8 stocks around 39 landfalls finds nothing: no abnormal return survives Holm adjustment, and the per-stock tests would detect a true 2% abnormal return 68 to 92% of the time for seven stocks and 18% for the eighth. A forecast-trigger trading rule loses 0.35% per event after assumed costs (cross-validated 95% interval -0.63% to -0.10%) and 0.15% before them, which cannot be told from zero. Published as a negative result; 40 of 40 deliberately injected bugs are caught by the tests.

## Data Science Projects and Research

### Galaxy Classification with Machine Learning and CNNs
[Repository](https://github.com/WilliamKwanProgramming/galaxy-classification-project)
STA496 Research Course under supervision of Prof. Antonio Martin at UofT Astrostatistics. Built regression models using astronomical feature extraction from more than 61000 galaxy images. This project implemented **Python**, and many of its data science libraries. Compared traditional machine learning methods to CNNs, and extracted embeddings using dimensionality reduction techniques. Finetuned ConvNext arch models for specfic classification tasks (ring galaxies, irregular galaxies, etc), and attained accuracy comparable to those of larger models.

### Global Economic Forecasting Platform
[Repository](https://github.com/WilliamKwanProgramming/macro-growth-forecast)
Global GDP Forecasting MLOps Pipeline is an end-to-end system that uses TensorFlow LSTMs and IMF World Economic Outlook data to forecast country-level GDP growth for 196 countries from 1980–2029. The project combines a Dockerized Airflow pipeline, DVC, and MLflow for automated data ingestion, training, experiment tracking, and versioning, with deployment via FastAPI and a Streamlit UI for interactive exploration of forecasts and model performance.

### GAN-Accelerated-Kinetic Monte Carlo
[Repository](https://github.com/WilliamKwanProgramming/GAN-Accelerated-Kinetic-Monte-Carlo)
Built a conditional GAN surrogate using Python for stochastic surface dynamics delivering 40x faster simulation than KMC while matching statistical targets; reproduced the codebase using data loaders, ResNet G/D, physics constraints, rollouts, logging to reproduce study results

### Derivative Pricing using Algorithms
[Repository](https://github.com/WilliamKwanProgramming/options-pricing-algorithm)
A self-contained library (plus Streamlit front-end) that prices European calls/puts, backs out implied volatility, and outputs the full Greek risk profile. Written from scratch in NumPy / SciPy, unit-tested for edge cases, and benchmarked against Bloomberg values to ±0.5 %. The app lets hiring managers plug in ticker-level inputs and see valuations, vol surfaces, and P/L heatmaps in seconds.

### RNN-Powered Quant Finance Document Classifier
[Repository](https://github.com/WilliamKwanProgramming/RNN-quant-document-classifer)
Bidirectional LSTM built with TensorFlow that ingests raw HTML filings and assigns them to Balance-Sheet, Cash-Flow, Income-Statement, Notes, or Other with 96 % test accuracy. A SMOTETomek pipeline fixes class imbalance; a Word2Vec embedding layer captures domain-specific vocabulary. Deployed as a Hugging Face Space via Streamlit so users can drop in a document and instantly get the label plus confidence score. Deployed as a streamlit app for ease of use.

### Stock Market Analysis and Prediction
[Repository](https://github.com/WilliamKwanProgramming/stock-data-analysis-prediction)
For my “Stock Market Analysis and Prediction” project, I tapped into The Investors Exchange (IEX) API to fetch live market data and performed comprehensive exploratory data analysis and visualization in Python. I developed techniques to assess a stock’s historical risk profile and then applied a Monte Carlo simulation to forecast its future price movements. Through this workflow, I combined real-time data processing, statistical modeling, and intuitive visualizations to uncover trends and quantify potential outcomes.

### AdventureWorks Sales Intelligence Dashboard
[Repository](https://github.com/WilliamKwanProgramming/adventure-works-sql-powerbi)
I extracted and cleaned the AdventureWorksDW2019 dataset using T-SQL in Microsoft SQL Server Management Studio, then exported the sanitized tables as CSVs. I enriched and modelled the data in Excel and Power Query before linking all tables into Power BI. Finally, I designed and published a three-page interactive dashboard highlighting overall sales trends, customer segmentation, and product performance, and also generated a static PDF report. Skills demonstrated: SQL, Excel, Power Query, data modelling, and Power BI visualization.

### Students Performance Predictor
[Repository](https://github.com/WilliamKwanProgramming/student-grade-predictor/)
Final project for DAT course at UofT. A Python-powered web app that predicts students’ math exam scores from demographic and academic factors. I built a robust preprocessing pipeline with scikit-learn’s ColumnTransformer to handle missing values and scale both numeric and categorical data, then trained and fine-tuned a regression model whose artifacts are loaded on demand in a Flask front end for instant predictions. The project includes interactive Jupyter notebooks for EDA and model diagnostics, and follows best practices for reproducibility with Conda environment management, Git version control, and clear modular code organization.

### Exploratory Data Analysis of Global Development Trends with Gapminder
[Repository](https://github.com/WilliamKwanProgramming/gapminder-analysis)
End-to-end R pipeline that pulls the 1952-2007 Gapminder dataset and walks it through a fully automated workflow: data wrangling with dplyr, 12 ggplot-driven visuals that track life-expectancy, GDP-per-capita and population trends, a log-linear regression linking economic growth to longevity, and a polished HTML report. Everything is scripted behind a Makefile, Bash helpers, and a Docker setup so hiring managers can reproduce the entire analysis with a single command.

### Spam Comments Detection with Machine Learning
[Repository](https://github.com/WilliamKwanProgramming/sta314_finalproject)

### Waste Classifier using Computer Vision
[Repository](https://github.com/WilliamKwanProgramming/computer-vision-waste-classification)

### TalkLikeMe: LLM Chat bot learned from your own texts
[Repository](https://github.com/WilliamKwanProgramming/ai-messaging-bot)

## Cybersecurity Projects

### Network Intrustion Detection
[Repository](https://github.com/WilliamKwanProgramming/network-intrustion-detection)

### Access Control Policy with AI
[Repository](https://github.com/WilliamKwanProgramming/access-control-policy-detection)

## Work / Research Experience
**Insurance-Linked Securities Analyst, Investment Management @ HOOPP (_Sept 2026 - Dec 2026_)**

- Build probabilistic hurricane-season forecast models that cut error 15% vs. a climatology baseline, scored by CRPS and Brier skill score in walk-forward backtests on 30 years of storm data
- Generate 3 trade recommendations (est. 40 bps spread pickup) from relative-value analysis of 25+ cat bonds using risk multiples, YTM, event-loss tables, AEP/OEP curves and stress scenarios
- Cut new-issuance screening time by 70% via Python/Snowflake ETL pipelines that parse offering documents and benchmark each cat bond against portfolio exposure, spread and expected loss
- Give PMs a same-day exposure view across 40+ cat bonds during active hurricanes by mapping live storm tracks to covered perils, regions and positions using RMS cat-model output
- Monitor VaR/TVaR and attachment/exhaustion probabilities across a \$1B+ cat bond and ILS fund portfolio

**Data Analyst Intern @ NAV CANADA (_May 2026 - Aug 2026_)**

- Improved revenue and demand forecast accuracy by 32% with ARIMA, SARIMAX and regression, informing \$1B revenue planning; cut data prep 85% via Databricks, PySpark and SQL pipelines over 2.4M+ records

**Business Analyst Intern @ Munich Re (_Jan 2026 - Apr 2026_)**

- Cut manual Excel pulls by 90% and saved underwriters 10+ hours/week with Power Automate reporting and a Power BI app; presented loss-ratio and exposure analyses to pricing teams covering a \$100M premium book

**ESOC Analyst Intern @ CIBC (_Sept 2025 - Dec 2025_)**

- Reduced false positives 10% and investigation time 15% via feature engineering and backtested anomaly scoring on Microsoft Sentinel, Defender and Proofpoint alerts; lifted reporting efficiency 20% with Python ETL

**Research Project @ University of Toronto (_June 2025 - August 2025_)**
[Repository](https://github.com/WilliamKwanProgramming/RqPINN-SciML-Algorithms-for-Eigenvalue-Problems)
- Built a physics-informed neural network (PINN) pipeline to solve the time-independent Schrödinger eigenproblem, implementing 4 complementary losses (PDE residual, normalization, eigenfunction orthogonality, monotone eigenvalue ordering) with autograd-based Laplacian and CUDA acceleration
- Engineered synthetic datasets via collocation sampling (LHC) and symmetry-aware model variants; built 8 Jupyter notebooks covering infinite/finite wells, harmonic oscillator, and multi-dimensional extension, with reusable training/evaluation utilities
- Validated models against close-form baselines (Predicted-vs-exact eigenpairs) and prototyped a variance-of-energy loss to improve multi-eigenstate training and reduce per-state retraining

**Research Assistant @ University of Toronto (_June 2024 - August 2024_)**
- Built a 320M record database tracking references to Google Books and OCLC using Python, SQL, 
BigQuery
- Engineered a parallel NLP pipeline using spaCy, NLTK, Regex that tagged 11M tech-year 
mentions with 92% precision and cut batch processing time by 25% through vectorization 
- Automated metadata scraping with BeautifulSoup, raising overall dataset completeness by 30%
- Analytical dashboard using PowerBI and Tableau

**Research Intern @ City University of Hong Kong (_June 2023 - August 2023_)**
- Built an end-to-end pipeline to generate PDE inverse-problem datasets (~500 train/test per run), train CNN / encoder-decoder models, and evaluate with finite-element norms (L2/H1) via Firedrake; fully scriptable CLI for reproducible experiments
- Coupled a differentiable PDE solver with PyTorch autograd to learn material parameters; trained up to 150 epochs with best-checkpoint selection by averaged L2 rel-error to 0.14 on a heat-conductivity benchmark
- Built an evaluation framework leveraging Firedrake’s function-space norms for rigorous model comparison
- Ensured reliability and contributions readiness with a Pytest test suite; aligned the example implementation with an ICLR 2023 paper reference to support physics-driven ML research 
