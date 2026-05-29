---
layout: post
title: "Dynamic Enforcement of Differential Privacy"
date: 2018-06-01 00:00:00 +0300
description: PhD thesis introducing new differential privacy backed frameworks, studying dynamic enforcement in both the centralised and local models. Chalmers University of Technology, 2018.
img: publications/HamidEbadi-PhDThesis-1.png
tags: [privacy, differential-privacy, formal-methods, programming-languages]
type: paper
venue: "PhD Thesis, Chalmers University of Technology (2018)"
authors: "Hamid Ebadi"
pdf: HamidEbadi-PhDThesis.pdf
---

**Authors:** Hamid Ebadi

**Venue:** Thesis for the Degree of Doctor of Engineering, Chalmers University of Technology, Göteborg, Sweden (2018)

## Abstract

With recent privacy failures in the release of personal data, differential privacy received considerable attention in the research community. This mathematical concept, despite its young age (Dwork et al., 2006), has grabbed the attention of many researchers for its robustness against identification of individuals even in presence of background information. Besides that, its flexible definition makes it compatible with different data sources, data mining algorithms and data release models. Its compositionality properties facilitate design of "differential privacy aware" programming languages and frameworks that empower non-experts to construct complex data mining analyses with proven differential privacy guarantees.

The goal of this research is to introduce new (and improve the current) differential privacy backed frameworks, prominent both in utility and flexibility of use. We study dynamic enforcement of differential privacy both in the *centralised model* in which a trusted curator process data stored in a centralised database and the *local model* with no trust on the third party.

For the centralised model the thesis mostly focuses on the privacy impact of the basic building blocks used in these frameworks, proving correctness of the system built upon them. With respect to accuracy, we present *"personalised differential privacy"* as an improved method of enforcing privacy that provides better data utilisation and other benefits. In this setting, individuals take control of their privacy requirements rather than being seen as a part of a database.

For the local model we propose a general framework in which the users can verify the received analyses and with a flexible policy express their privacy preference in different forms such as enforcing their personalised privacy budget.

## Citation

> Ebadi, H. (2018). *Dynamic Enforcement of Differential Privacy*. PhD Thesis, Chalmers University of Technology.

<a href="/Publications/HamidEbadi-PhDThesis.pdf" class="download-btn" download><i class="fa fa-file-pdf-o"></i> Download PDF</a>
<a href="/Publications/HamidEbadi-PhDThesis.bib" class="download-btn download-btn--bib" download><i class="fa fa-quote-right"></i> Download BibTeX</a>
