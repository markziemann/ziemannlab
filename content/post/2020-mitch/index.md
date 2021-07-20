---
date: "2020-06-29T13:09:13-06:00"
author: "Mark Ziemann"
title: Multi-contrast enrichment with mitch
---

<img src="https://github.com/markziemann/mitch_paper/raw/master/figs/mitch.png" alt="drawing" style="width:200px;"/>

Pathway enrichment analysis is among the most frequently used types of computational biology analysis, enabling us to better interpret and summarise massive gene regulation datasets into a manageable list of pathways.

While this is truly powerful, most pathway analysis tools are limited to a single comparison, which is a problem if the dataset consists of multiple sample groups, for example if we are working with an multiple disease and treatment groups, as tends to be the case for most omics experiments undertaken these days.

Standard single contrast techniques like DAVID or GSEA can be used multiple times, but this decreases the ability to identify subtle patterns of regulation over multiple contrasts. 

[Cox and Mann (2012)](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-13-S16-S12) proposed the use of the MANOVA test for enrichment analysis of multiple contrasts, but there were a few drawbacks; (i) the software was not interoperable with the R/bioconductor workflows used in genomics, and (ii) the analysis was limited to only one or two dimensions.

To address this Dr Antony Kaspi (now based at WEHI) drafted R codes that would enable MANOVA-powered gene set enrichment analysis. Dr Kaspi and the team of Prof Sam El-Osta used the functions extensively in the period 2014-2018 for a variety of omics analysis projects in diabetes, epilepsy and heart development.

As the software was central for the success of a number of projects, Drs Kaspi and Ziemann decided to formalise the code into a Bioconductor package. 

The package was accepted into Bioconductor in December 2019, and the journal article appeared in *BMC genomics* in the following June [(Kaspi & Ziemann 2020)](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-020-06856-9).

In terms of downloads, the mitch package ranks in the top 900 Bioconductor packages and is still under active development.
Our group uses mitch heavily in our collaborative work, and we routinely help other groups develop their mitch-based enrichment analysis workflows.

### References

Cox, J. and Mann, M. (2012) “1D and 2D annotation enrichment: a statistical method integrating quantitative proteomics with complementary high-throughput data,” BMC bioinformatics, 13 Suppl 16(S16), p. S12.

Kaspi, A. and Ziemann, M. (2020) “Mitch: Multi-contrast pathway enrichment for multi-omics and single-cell profiling data,” BMC genomics, 21(1), p. 447.

### Some of the projects that have used mitch

Sim, C. B. et al. (2021) “Sex-specific control of human heart maturation by the progesterone receptor,” Circulation, 143(16), pp. 1614–1628.

Tan, S. M. et al. (2021) “Targeting methylglyoxal in diabetic kidney disease using the mitochondria-targeted compound MitoGamide,” Nutrients, 13(5). doi: 10.3390/nu13051457.

Watt, K. I. et al. (2021) “Yap regulates skeletal muscle fatty acid oxidation and adiposity in metabolic disease,” Nature communications, 12(1), p. 2887.