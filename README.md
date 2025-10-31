# Data Scientist/Statistician

#### Technical Skills: Python, R, SQL, Excel, MATLAB, Adobe Suite (AutoCAD, Acrobat), Microsoft Office, LaTeX, Linux, Networking

## Education
- M.S., Statistics | University of Toronto (_June 2027_)
- B.S., Mathematics and Statistics | University of Toronto (_June 2025_)

## Work / Research Experience
**ESOC Analyst Intern @ CIBC (_Sept 2025 - Dec 2025_)**

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


## Data Science Projects and Research
### Galaxy Classification with Machine Learning and CNNs
[Repository](https://github.com/WilliamKwanProgramming/galaxy-classification-project)
STA496 Research Course under supervision of Prof. Antonio Martin at UofT Astrostatistics. Built regression models using astronomical feature extraction from more than 61000 galaxy images. This project implemented **Python**, and many of its data science libraries. Compared traditional machine learning methods to CNNs, and extracted embeddings using dimensionality reduction techniques. Finetuned ConvNext arch models for specfic classification tasks (ring galaxies, irregular galaxies, etc), and attained accuracy comparable to those of larger models. 

### GAN-Accelerated-Kinetic Monte Carlo
[Repository](https://github.com/WilliamKwanProgramming/GAN-Accelerated-Kinetic-Monte-Carlo)
Built a conditional GAN surrogate using Python for stochastic surface dynamics delivering 40x faster simulation than KMC while matching statistical targets; reproduced the codebase using data loaders, ResNet G/D, physics constraints, rollouts, logging to reproduce study results

### RNN-Powered Quant Finance Document Classifier
[Repository](https://github.com/WilliamKwanProgramming/RNN-quant-document-classifer)
Bidirectional LSTM built with TensorFlow that ingests raw HTML filings and assigns them to Balance-Sheet, Cash-Flow, Income-Statement, Notes, or Other with 96 % test accuracy. A SMOTETomek pipeline fixes class imbalance; a Word2Vec embedding layer captures domain-specific vocabulary. Deployed as a Hugging Face Space via Streamlit so users can drop in a document and instantly get the label plus confidence score. Deployed as a streamlit app for ease of use. 

### AdventureWorks Sales Intelligence Dashboard
[Repository](https://github.com/WilliamKwanProgramming/adventure-works-sql-powerbi)
I extracted and cleaned the AdventureWorksDW2019 dataset using T-SQL in Microsoft SQL Server Management Studio, then exported the sanitized tables as CSVs. I enriched and modelled the data in Excel and Power Query before linking all tables into Power BI. Finally, I designed and published a three-page interactive dashboard highlighting overall sales trends, customer segmentation, and product performance, and also generated a static PDF report. Skills demonstrated: SQL, Excel, Power Query, data modelling, and Power BI visualization.

### Students Performance Predictor
[Repository](https://github.com/WilliamKwanProgramming/student-grade-predictor/)
Final project for DAT course at UofT. A Python-powered web app that predicts students’ math exam scores from demographic and academic factors. I built a robust preprocessing pipeline with scikit-learn’s ColumnTransformer to handle missing values and scale both numeric and categorical data, then trained and fine-tuned a regression model whose artifacts are loaded on demand in a Flask front end for instant predictions. The project includes interactive Jupyter notebooks for EDA and model diagnostics, and follows best practices for reproducibility with Conda environment management, Git version control, and clear modular code organization.

### Derivative Pricing using Algorithms
[Repository](https://github.com/WilliamKwanProgramming/options-pricing-algorithm)
A self-contained library (plus Streamlit front-end) that prices European calls/puts, backs out implied volatility, and outputs the full Greek risk profile. Written from scratch in NumPy / SciPy, unit-tested for edge cases, and benchmarked against Bloomberg values to ±0.5 %. The app lets hiring managers plug in ticker-level inputs and see valuations, vol surfaces, and P/L heatmaps in seconds. 

### Stock Market Analysis and Prediction
[Repository](https://github.com/WilliamKwanProgramming/stock-data-analysis-prediction)
For my “Stock Market Analysis and Prediction” project, I tapped into The Investors Exchange (IEX) API to fetch live market data and performed comprehensive exploratory data analysis and visualization in Python. I developed techniques to assess a stock’s historical risk profile and then applied a Monte Carlo simulation to forecast its future price movements. Through this workflow, I combined real-time data processing, statistical modeling, and intuitive visualizations to uncover trends and quantify potential outcomes.

### Spam Comments Detection with Machine Learning
[Repository](https://github.com/WilliamKwanProgramming/sta314_finalproject)

### Exploratory Data Analysis of Global Development Trends with Gapminder
[Repository](https://github.com/WilliamKwanProgramming/gapminder-analysis)
End-to-end R pipeline that pulls the 1952-2007 Gapminder dataset and walks it through a fully automated workflow: data wrangling with dplyr, 12 ggplot-driven visuals that track life-expectancy, GDP-per-capita and population trends, a log-linear regression linking economic growth to longevity, and a polished HTML report. Everything is scripted behind a Makefile, Bash helpers, and a Docker setup so hiring managers can reproduce the entire analysis with a single command.


### Waste Classifier using Computer Vision
[Repository](https://github.com/WilliamKwanProgramming/computer-vision-waste-classification)


### TalkLikeMe: LLM Chat bot learned from your own texts
[Repository](https://github.com/WilliamKwanProgramming/ai-messaging-bot)

## Cybersecurity Projects

### Network Intrustion Detection
[Repository](https://github.com/WilliamKwanProgramming/network-intrustion-detection)

### Access Control Policy with AI
[Repository](https://github.com/WilliamKwanProgramming/access-control-policy-detection)

