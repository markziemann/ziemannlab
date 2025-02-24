---
title: "Available Shiny Tools"
date: '2023-08-04'
---

# LAM: improved pathway enrichment tool for Infinium methylation data

This is a novel pathway enrichment tool specifically for methylation array data.
It is similar to GSEA, but uses a clever way to aggregate methylation measurements
at CpG sites to the gene level.
This tool can be run on our web server, or if you have docker on your computer
you can run it yourself and get results faster.

* On the web: [Launch app](https://lam.ziemann-lab.net)

* Run it on your own hardware: [GitHub](https://github.com/markziemann/gmea_app)

For information about the method, please refer to the [publication](https://doi.org/10.1080/15592294.2024.2375022).

Ziemann M, Abeysooriya M, Bora A, Lamon S, Kasu MS, Norris MW, Wong YT, Craig JM. Direction-aware functional class scoring enrichment analysis of infinium DNA methylation data. Epigenetics. 2024 Dec;19(1):2375022. doi: 10.1080/15592294.2024.2375022. Epub 2024 Jul 5. PMID: 38967555.

# ORA: Investigating two subtle problems with over-representation analysis

We know that some enrichment tools produce different results with the same input
data.
In this work we found and characterised two subtle issues.
The first one is the improper handling of background genes, and the second one
is improper false discovery rate control.
You can input your data into this tool and it will show you how these two problems
can distort your results.

* On the web: [Launch app](https://oratool.ziemann-lab.net)

* Run it on your own hardware: [GitHub](https://github.com/markziemann/background?tab=readme-ov-file#shiny-app)

For information about the method, please refer to the [publication](https://doi.org/10.1093/bioadv/vbae159)

Ziemann M, Schroeter B, Bora A. Two subtle problems with overrepresentation analysis. Bioinform Adv. 2024 Oct 21;4(1):vbae159. doi: 10.1093/bioadv/vbae159. PMID: 39539946; PMCID: PMC11557902.
