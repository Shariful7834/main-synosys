---
title: "Causal Inference in Pandemic Time Series"
subtitle: "Understanding the temporal evolution of COVID-19"
abstract: ""

authors:
  - adrianp

tags:
 - causal inference
 - nonlinear dynamics
 - COVID-19
 - pandemic
 - mobility

summary: ""

categories: []
date: "2024-09-02"

lastMod: "2024-09-02"

featured: false

draft: true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
caption: ""
focal_point: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.

---

Naturally emerging phenomena, such as the COVID-19 pandemic, cannot be studied in controlled experiments with "laboratory" settings. This makes it all the more important to investigate the complex relationships between empirically observable variables in order to understand the driving forces. 

Here, we are interested in the time lagged linear and nonlinear causal relationships between multiple time series variables originating from the 38 *nomenclature of territorial units for statistics* (*NUTS2*) regions constituting Germany, where we believe that all of these time series contribute to the temporal evolution of COVID-19 within said region. These variables are for example the daily temperature ($W$), representing an environmental driver, several mobility time series such as the daily influx mobility ($J$), the daily inner mobility ($J^{in}$) and the contact index ($CX$), as well as a representative of the temporal evolution of COVID-19, here, the approximated reproduction rate ($A$). 



Three methods are applied, that is the time lagged cross-correlation, time lagged partial cross-correlation and time lagged cross-mapping, which is rooted in state space reconstruction. 

On a NUTS2 scale, mobility is always driven by daily temperature. In most cases mobility also drives the reproduction rate with longer time lags, while the reproduction rate influences mobility with shorter time lags. Together, these results show the importance of differentiated analysis based on the geographic location of the data generating process.
