---
title: Predicting Phenotype from Genomic Sequence with Deep Neural Networks
summary: "Predicting pairwise gene interactions using attention-based RNN/CNN, and compared to baseline approach with 
random forest procedure with gene ontotype described in [Yu, et al. (Cell Systems, 2016)](http://www.cell.com/cell-systems/abstract/S2405-4712(16)30033-3) 
on the *S. cerevisiae* data from [Costanzo, et al. (Science, 2010)](http://science.sciencemag.org/content/327/5964/425.long)."

tags:
- Deep Learning
date: "2018-01-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Genome representation
  focal_point: Smart

links:
url_code: ""
url_slides: "/project/example/genome_prediction.pdf"
url_pdf: "/project/example/gi_project_wli.pdf"
url_video: ""


# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

---
## Summary
In Yu M. et al. (2016), phenotype is translated from genotype based on gene ontology, and predicted interaction scores 
may be influenced by errors in gene annotations or relationship between terms. As deep learning being effective in 
identifying complex patterns from feature-rich datasets, especially as recurrent neural networks(RNNs) such as long 
short term memory(LSTM) and gated recurrent unit(GRU) are capable of dealing with long-distance sequential data, 
predicting genetic interactions directly from DNA or amino-acid sequences using deep learning techniques would help us 
gain insights into underlying complex phenotypes.
