![R](https://img.shields.io/badge/R-4.4.0-blue?logo=r)
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![License](https://img.shields.io/github/license/celsomsilva/thesis-data-science-usp)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)



# Walmart Sales Prediction - HLM3 (Machine Learning Multilevel Modeling) - 2023/2024

This repository contains my thesis project, where I analyze the factors influencing Walmart's weekly sales using **multilevel modeling (HLM3)**, a **machine learning approach** for hierarchical data, and compare it against traditional **generalized linear models (GLM)**.
The work demonstrates the effectiveness of **nonlinear hierarchical models** in **predicting sales**, particularly when the data is structured across multiple levels.



---

## Evaluation

- **Grade:** 9.0 (University of São Paulo - USP, 2024)  
- **Committee feedback:** *"Interesting and challenging."*  

---

## Repository Status

This repository is **work-in-progress**.  
Current focus:  
- Organizing and documenting codes and papers
- Translating the thesis and more (Portuguese → English)  


Planned:  
- Publishing code and documents in this repository
- Possible future integration with Deep Learning
- Extending version with analytics & storytelling 

---


## Important

USP employs institutional similarity detection tools such as Turnitin / SimilarityCheck, which compare documents against extensive academic databases, repositories, and publicly available web content. Any claims of authorship or originality can therefore be officially verified by the university.

It is worth noting that even texts produced with the aid of artificial intelligence, once published on repositories or web pages, can be detected by similarity tools. Moreover, faculty evaluation considers writing style, methodological consistency, and coherence between analysis, code, and results — ensuring that only genuinely original work is approved.

---


## Extended Version with Analytics & Storytelling

This repository contains the **academic/technical version** of my undergraduate thesis,  
focused on multilevel statistical modeling (HLM3) applied to Walmart's weekly sales.  
Here you will find only the **R code** (**python** in the near future) and the **figures used in the thesis document**.

For a more **didactic and applied version**, with emphasis on **analytics, storytelling, and communication of insights**,  
please check the complementary repository:

[Analytics & Storytelling Repository](https://github.com/celsomsilva/thesis-storytelling-usp)

---

## Abstract
The main objective of this thesis is to analyze the factors that influence Walmart's weekly sales using Machine Learning techniques with a statistical focus.  
A **nonlinear 3-level Hierarchical Linear Model (HLM3)** was developed and compared step by step with equivalent **Generalized Linear Models (GLM)** that do not account for random effects.  

The modeling process included:
- Null models for linear regression, nonlinear regression with **Yeo-Johnson transformation**, and multilevel HLM3 (linear and nonlinear).
- Full models for linear and nonlinear regression.
- Performance evaluation using **Log-Likelihood (LogLik)**, **Akaike’s Information Criterion (AIC)**, and **Bayesian Information Criterion (BIC)**.  

The study shows that **multilevel modeling is a promising approach** for handling hierarchically distributed data and can provide valuable insights for sales strategies and decision-making.  
The results contribute to the statistical understanding of hierarchical modeling and provide a foundation for future research in this area.

**Keywords:** Box-Cox, Yeo-Johnson, Multilevel Model, Hierarchical Model, Machine Learning

---

## Project Structure
```

walmart-sales-hlm3/
│── src/
│   ├── varejo_multinivel_hlm3.R
│   ├── modelagem_multinivel.ipynb
│   ├── tratamento_de_dadosfinal.ipynb
│
│── data/
│   └── varejo_hlm_ready.csv
│
│── docs/
│   ├── TCC_REVISADO.pdf
│   ├── Apresentacao.pdf
│   └── images/
│       ├── aic_bic.png
│       ├── boxplot.png
│       └── ...
│
│── .gitignore
│── README.md
│── LICENSE (optional)

```

---

## Models Used
- GLM (Generalized Linear Models)
- HLM3 (3-Level Hierarchical Linear Models – linear and nonlinear)
- Transformations: Yeo-Johnson, Box-Cox
- Statistical comparison: LogLik, AIC, BIC

---

## How to Reproduce
1. Install the required R packages (`lme4`, `car`, `ggplot2`, etc.).
2. Preprocess the data (already done in `src/tratamento_de_dadosfinal.ipynb`) or use `data/varejo_hlm_ready.csv` directly.
3. Open `src/varejo_multinivel_hlm3.R` to run the full analysis, using RStudio.
4. Alternatively, use `src/modelagem_multinivel.ipynb` in Jupyter Notebook for an exploratory workflow.

---

## Documentation
- [`docs/TCC_REVISADO.pdf`](docs/TCC_REVISADO.pdf) – Final version of the thesis (Portuguese).
- [`docs/Apresentacao.pdf`](docs/Apresentacao.pdf) – Presentation slides (Portuguese).
- [`docs/images/`](docs/images/) – Figures used in the thesis and slides.

---


## About the Author

I’m a Data Science and Analytics specialist (USP postgraduate) and Computer Engineer (UERJ) with a career spanning from **Pascal/C/Java roots** to **modern Machine Learning and AI**.

My academic and professional background includes:

* **Computation in general**
* **Machine Learning**
* **Hierarchical nonlinear mixed models (HLM3/HLM2)**, **Intraclass correlation (ICC)** and other topics about **HLM**
* **Residual diagnostics and model validation**
* **Deep Learning, LLMs, and Reinforcement Learning (ongoing specialization)**

---

## Contact  

- [LinkedIn](https://linkedin.com/in/celso-m-silva)  
- Or open an [issue](https://github.com/celsomsilva/thesis-data-science-usp/issues)

