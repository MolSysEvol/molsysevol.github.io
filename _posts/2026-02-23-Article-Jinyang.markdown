---
layout: post
title: "New publication out: SNP polarization with the ARG"
date: 2026-02-23 18:20:00 -0000
categories: Publication
---


Jinyang's paper is out: [DOI: 10.1111/1755-0998.70105](https://doi.org/10.1111/1755-0998.70105)

In this work, we describe a new method to polarize SNPs (that is, inferring which allele is ancestral).
We developped a maximum likelihood procedure to compute the probabilities of ancestral states. Briefly, we show that

* When the ARG is known and the mutation did not occur on one of the root branches, we can recover the ancestral allele with 100% accuracy
* When the ARG is known and the mutation occurred on one of the root branches and the mutation is neutral, the posterior probability contains information on the ancestral state, which allow to recover the site frequency spectrum without bias
* When the ARG is not know, results differ a lot depending on the method employed. Surprisingly, we found out that the most accurate approach is to infer pairwise TMRCAs using a PSMC method, and then reconstruct local genealogies using UPGMA.
* Selection has a non-straightforward impact on the results. Linked selection has no direct consequence: when the marginal genealogy is known or accurately inferred, the reconstruction a linked sites is unbiased. However, the selected mutation itself will not be properly polarized in case it occurred at one of the root branches. In such case, the likelihood calculation is incorrect because of model violation, which leads to inaccurate posterior probabilities.

We called this new method **PolarBEAR**, for **Polar**ization **B**y **E**stimation of the **A**ncestral **R**ecombination Graph. We posit that it will prove useful in many cases where no outgroup sequence is available for population genomic inference.

 

