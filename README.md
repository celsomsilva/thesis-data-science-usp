# Walmart Sales Prediction – HLM3 (Hierarchical Models, Nonlinear)

> “A data scientist is not a button pusher.” — Prof. Luiz Paulo Fávero

This repository contains my thesis project, where I analyze Walmart’s weekly sales data using **3-level hierarchical models (HLM3)** and compare them with **generalized linear models (GLMs)** that ignore the data hierarchy.
The goal was to understand what drives weekly sales and to show how **nonlinear multilevel models** can outperform traditional approaches when the data is naturally nested (Store → Department → Week).

---

## Evaluation

* **Grade:** 9.0 (University of São Paulo – USP, 2024)
* **Committee feedback:** *“Interesting and challenging.”*

---

## Project Status

Work in progress — I continue to improve documentation, figures, and comparisons.

---

## Academic Note

USP uses official similarity-checking systems (Turnitin / SimilarityCheck).
All thesis submissions are automatically verified against academic databases and public sources.
Even AI-generated text becomes traceable once published online.

The evaluation considers writing consistency, methodology, and whether the code, analysis, and text form a coherent whole — meaning only genuinely original work passes.

---

## Extended Versions

If you want a more **applied**, **storytelling**, or **analytics-focused** version of this project:

**Analytics & Storytelling repo:**
[https://github.com/celsomsilva/thesis-storytelling-usp](https://github.com/celsomsilva/thesis-storytelling-usp)

**Quarto website version:**
[https://github.com/celsomsilva/walmart-analytics-storytelling](https://github.com/celsomsilva/walmart-analytics-storytelling)

---

## Abstract

This thesis analyzes the factors that influence Walmart’s weekly sales using statistical machine learning techniques.
A **nonlinear 3-level HLM (HLM3)** was built and compared with several **GLM-based models**, including versions with and without transformations (Box-Cox/Yeo-Johnson) and negative binomial alternatives.

The workflow included:

* Null vs full models (GLM and multilevel)
* Linear and nonlinear setups
* Yeo–Johnson transformation for stabilizing variance
* Negative binomial models for overdispersed data
* Model comparison using **LogLik, AIC, BIC**

The results consistently show that:

* **Hierarchical models fit the data structure better**
* **Predictions improve** when store and department effects are modeled
* **Interpretation becomes clearer** for decision-making

This contributes both to statistical understanding of HLMs and to practical retail insights.

**Keywords:** Multilevel models, Yeo–Johnson, Box-Cox, HLM3, hierarchical data, machine learning

---

## Models Included

The initial HLM/OLS templates were provided in class by Prof. Fávero (HTML2/HTML3 exercises).
This project expands those ideas by adding:

* GLMs and GLMMs
* Negative binomial and multilevel negative binomial models
* Nonlinear transformations (Yeo–Johnson)
* Full diagnostics and comparative modeling

---

## Figures

Some reference figures come from class material;
all extended visualizations (AIC/BIC charts, residual diagnostics, multilevel diagrams, etc.) were created for the thesis.

---

## Project Structure

```
walmart-sales-hlm3/
  src/
    varejo_multinivel_hlm3.R
    modelagem_multinivel.ipynb
    tratamento_de_dadosfinal.ipynb

  data/
    varejo_hlm_ready.csv

  docs/
    TCC_REVISADO.pdf
    Apresentacao.pdf
    images/
      aic_bic.png
      boxplot.png
      ...

  .gitignore
  README.md
  LICENSE               # MIT
  LICENSE-thesis.txt    # Creative Commons (thesis)
```

---

## How to Reproduce

1. Install R packages (`lme4`, `car`, `ggplot2`, etc.)
2. Use the ready dataset (`data/varejo_hlm_ready.csv`) or preprocess it using
   `src/tratamento_de_dadosfinal.ipynb`
3. Run the full analysis in
   `src/varejo_multinivel_hlm3.R`
4. Or explore the notebook version:
   `src/modelagem_multinivel.ipynb`

---

## Documentation

* **Thesis (Portuguese):**
  [`docs/TCC_REVISADO.pdf`](docs/TCC_REVISADO.pdf)

* **Presentation slides (Portuguese):**
  [`docs/Apresentacao.pdf`](docs/Apresentacao.pdf)

English versions coming soon:

* `docs/en/Thesis_final.pdf`
* `docs/en/Presentation.pdf`

Figures used in the thesis are under `docs/images/`.

---


## Author

This project was developed by an engineer and data scientist with a background in:

* Postgraduate degree in **Data Science and Analytics (USP)**
* Bachelor's degree in **Computer Engineering (UERJ)**
* Special interest in statistical models, interpretability, and applied AI

---


## Acknowledgments

- Prof. Delmo Alves de Moura (UFABC) — for his guidance and support throughout my thesis
- Prof. Luiz Paulo Fávero (USP) — for emphasizing deep statistical foundations


---

## License

- The source code in this repository is licensed under the [MIT License](./LICENSE).
- The thesis document is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](./LICENSE-thesis.txt).

---

## Contact  

- [LinkedIn](https://linkedin.com/in/celso-m-silva)  
- Or open an [issue](https://github.com/celsomsilva/thesis-data-science-usp/issues)

