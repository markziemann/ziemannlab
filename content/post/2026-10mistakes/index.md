---
title: "Now published: Ten common mistakes that could ruin your enrichment analysis"
author: "Mark Ziemann"
date: 2026-04-23
categories: ["Reproducibility","Life Science","Bioinformatics","Pathway analysis","Enrichment analysis"]
tags: ["Deakin","Burnet"]
---

![Common enrichment tool logos: DAVID, GSEA, ClusterProfiler, KEGG, IPA, GeneOntology](enrichment.png)

Glad to share with you our published article [*Ten common mistakes that could ruin your enrichment analysis*](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1014122). 
The work was done by Anusuiya Bora (Burnet Bioinformatics, Deakin Uni), Matthew McKenzie (Deakin) and I.

My working group got interested into pathway enrichment analysis in around 2020/2021 because I was receiving review requests
for manuscripts and many of them suffered from severe problems, leading me to believe that these issues were prevalent.
Our first article on this theme [Wijesooriya et al, 2022](https://doi.org/10.1371/journal.pcbi.1009935) demonstrated that
severe problems were really common across a big sample of peer-reviewed articles including:

1. Lack of p-value correction.

2. Wrong background list.

3. Lack of methodological details.

We showed that problems 1 and 2 led to dramatic biases in results that could alter the conclusions of transcriptome studies.
Due to reviewer disagreements, we were unable to provide a more comprehensive set of best practices in that article, but this
remained a priority of ours, especially given that many of the existing recommendations articles actually misses some of the 
most crucial problems.
For example the [Chicco and Agapito 2022](https://doi.org/10.1371/journal.pcbi.1010348) aricle missed the background problem.

During the past few years, we developed a deeper understanding of the various enrichment tools and their strengths and weaknesses,
including identifying some bugs in some over-representation tools [Ziemann et al, 2024](https://doi.org/10.1093/bioadv/vbae159).

This lead us to identify some other less common issues that enrichment users should be aware of. 
These recommendations are based on empirical data. 
Throughout this new article, we use simulated and real transcriptome data to demonstrate the impact of these errors.

I hope this is a turning point in pathway enrichment and bioinformatics in general.
We should no longer be tolerating sloppy analysis and reporting.
Our funders deserve better than to have expensive omics studies undermined by flawed enrichment analysis.