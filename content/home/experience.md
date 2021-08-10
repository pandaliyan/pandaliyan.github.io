---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 20

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Senior Machine Learning Research Engineer (NLP)
    company: Comcast Applied AI Research Lab
    company_url: 'https://jobs.comcast.com/ml-ai-team-page'
    company_logo: ''
    location: Washington D.C.
    date_start: '2019-01-01'
    date_end: '2021-07-23'
    description: |2-
        * Designed an unsupervised auto-annotation and active learning pipeline which used user behavioral modeling to automatically
          identify errors in speech recognition and NLP systems and suggest corrections; summarized the work into a
          conference paper as the first-author and filed a patent as main contributor
        * Developed a context-based approach that discovered misclassified user queries in question answering systems by
          performing semantic search with Sentence-BERT and clustering
        * Leveraged subword-level query representation and adversarial training in customer care dialogue system for
          misspelled user queries, which improved classification accuracy by 18% and increased user experience stability
    

design:
  columns: '2'
---
