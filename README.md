# 🔬 Sci-Viz Lab

*A curated collection of reproducible, publication-ready plotting recipes in **Python** and **R***  
designed for researchers who need **beautiful** and **rigorous** figures—quickly.

<div align="center">
  <img src="https://img.shields.io/badge/build-passing-brightgreen" />
  <img src="https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue" />
  <img src="https://img.shields.io/badge/R-≥4.2-blueviolet" />
  <img src="https://img.shields.io/badge/license-MIT-lightgrey" />
</div>

---

## ✨ What’s inside?

| Tier | Figure families | Typical use-case |
|------|-----------------|------------------|
| **📊 Basic Charts** | Area • Bar • Line / Scatter • Box • Polar • Simple Network | quick looks at distributions, trends, or category comparisons |
| **📈 Advanced Charts** | Heatmap • Violin • Venn • Cluster dendrogram • Significance plots • Enrichment plots • Dim-red (PCA, t-SNE, UMAP) • Regression (fit curves, residual) • Correlation matrices • ML diagnostics (feature importance, ROC, decision tree) | conference slides • journal figures • technical proposals |

Every notebook / script is crafted to be:

* **Self-contained** – just run and it works (sample data included or fetched).
* **Style-aware** – sane defaults: LaTeX labels, colour-blind palettes, dpi ≥ 300.
* **Tweak-friendly** – key parameters exposed at the top; no digging through code.

---

## 🗂 Repository layout
Sci-Viz Lab/
├── python/
│ ├── basic/
│ │ ├── bar_chart.ipynb
│ │ └── line_scatter.ipynb
│ ├── advanced/
│ │ ├── heatmap.ipynb
│ │ └── pca_umap.ipynb
│ └── utils/ # common styling helpers
├── R/
│ ├── basic/
│ ├── advanced/
│ └── utils/
└── data/ # lightweight demo datasets


> **Why both languages?**  
> Python notebooks rely on *Matplotlib / Seaborn / Plotly / scikit-learn*.  
> R scripts leverage *ggplot2 / ComplexHeatmap / cluster / caret*… choose what fits your stack.

---

## 🚀 Quick start

```bash
# clone
git clone https://github.com/<your-user>/sci-viz-lab.git
cd sci-viz-lab

# Python environment
conda env create -f python/environment.yml
conda activate sci-viz

# launch examples
jupyter lab python/basic/bar_chart.ipynb

#For R users:
install.packages(c("tidyverse", "ggplot2", "ComplexHeatmap", "umap", "cluster"))
# then open R/basic/heatmap.Rmd in RStudio and knit

