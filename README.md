![R](https://img.shields.io/badge/R-4.4.0-blue?logo=r)
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![License](https://img.shields.io/github/license/celsomsilva/thesis-data-science-usp)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)



# Walmart Sales Prediction - HLM3 (Hierarchical Linear Models) Non Linear

This repository contains my thesis project, where I analyze the factors influencing Walmart's weekly sales using **multilevel modeling (HLM3)**, a **machine learning approach** for hierarchical data, and compare it against traditional **generalized linear models (GLM)**.
The work demonstrates the effectiveness of **nonlinear hierarchical models** in **predicting sales**, particularly when the data is structured across multiple levels.

---

## Evaluation

- **Grade:** 9.0 (University of São Paulo - USP, 2024)  
- **Committee feedback:** *"Interesting and challenging."*  

---

## Repository Status

This repository is a **work in progress**. Current focus includes:  
- Organizing and documenting code, datasets, and figures  
- Gradually translating thesis sections **from Portuguese to English**  
- Refining structure for clarity and reproducibility  

Planned next steps:  
- Publishing all code and supporting documents in this repository  
- Extending model comparisons with **Deep Learning** and 
- Developing a parallel version focused on **analytics & storytelling** 


---


## Important

USP employs institutional similarity detection tools such as Turnitin / SimilarityCheck, which compare documents against extensive academic databases, repositories, and publicly available web content. Any claims of authorship or originality can therefore be officially verified by the university.

It is worth noting that even texts produced with the aid of artificial intelligence, once published on repositories or web pages, can be detected by similarity tools. Moreover, faculty evaluation considers writing style, methodological consistency, and coherence between analysis, code, and results — ensuring that only genuinely original work is approved.

---


## Extended Version with Analytics & Storytelling

For a more **didactic and applied version**, with emphasis on **analytics, storytelling, and communication of insights**,  
please check the complementary repository:

[Analytics & Storytelling Repository](https://github.com/celsomsilva/thesis-storytelling-usp)

---

## Abstract

This thesis aims to analyze factors influencing Walmart's weekly sales using Machine Learning techniques with a statistical focus. A **nonlinear 3-level Hierarchical Linear Model (HLM3)** was developed and compared step-by-step with equivalent **Generalized Linear Models (GLM)** that do not incorporate random effects.

The modeling process included:

- Null and full models for **GLM and multilevel approaches**, including linear regression, nonlinear regression with **Yeo-Johnson transformation**, and Multilevel Negative Binomial models.
- Evaluation metrics such as **Log-Likelihood (LogLik)**, **Akaike Information Criterion (AIC)**, and **Bayesian Information Criterion (BIC)**.

Results show that multilevel models better capture hierarchical patterns, improving prediction accuracy and interpretability for decision-making. This study demonstrates that **multilevel modeling is a promising approach** for hierarchically structured data and provides valuable insights for sales strategies.

These findings contribute to the statistical understanding of hierarchical models and offer a foundation for future research.

**Keywords:** Box-Cox, Yeo-Johnson, Multilevel Model, Hierarchical Model, Machine Learning


---

## Models

The original linear HLM and OLS scripts were provided as exercises by Prof. Fávero, USP.  
This project significantly extends the original scope, implementing a suite of models including GLMs, GLMMs, negative binomial models, multilevel extensions, and various transformations for model comparison.

---

## Figures

Some figures are adapted from materials provided by Prof. Fávero, USP (HTML2/HTML3 exercises).  
All other figures, including adaptations and new visualizations for binomial negative and multilevel models, were created by the author.
 

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

## How to Reproduce
1. Install the required R packages (`lme4`, `car`, `ggplot2`, etc.).
2. Preprocess the data (already done in `src/tratamento_de_dadosfinal.ipynb`) or use `data/varejo_hlm_ready.csv` directly.
3. Open `src/varejo_multinivel_hlm3.R` to run the full analysis, using RStudio.
4. Alternatively, use `src/modelagem_multinivel.ipynb` in Jupyter Notebook for an exploratory workflow.

---

## Documentation


- [`docs/pt/TCC_REVISADO.pdf`](docs/pt/TCC_REVISADO.pdf) – Final thesis *(in Portuguese)*  
- [`docs/pt/Apresentacao.pdf`](docs/pt/Apresentacao.pdf) – Defense presentation slides *(in Portuguese)*  

*(Coming soon: English versions)*  
- [`docs/en/Thesis_final.pdf`](docs/en/Thesis_final.pdf) – Final thesis *(in English)*  
- [`docs/en/Presentation.pdf`](docs/en/Presentation.pdf) – Defense presentation slides *(in English)*

- [`docs/images/`](docs/images/) – Figures used in thesis.  

---


## About the Author

I’m a Data Science and Analytics specialist (USP postgraduate) and Computer Engineer (UERJ) with a career spanning from **Pascal/C/Java roots** to **modern Machine Learning and AI**.

My academic and professional background includes:

- **Computation in general**
- **Machine Learning**
- **Hierarchical nonlinear mixed models (HLM3/HLM2)**, **Intraclass correlation (ICC)** and other topics about **HLM**
- **Residual diagnostics and model validation**
- **Deep Learning, LLMs, and Reinforcement Learning (ongoing specialization)**

---

## License

- The source code in this repository is licensed under the [MIT License](./LICENSE).
- The thesis document is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](./LICENSE-thesis.txt).

---

## Contact  

- [LinkedIn](https://linkedin.com/in/celso-m-silva)  
- Or open an [issue](https://github.com/celsomsilva/thesis-data-science-usp/issues)

