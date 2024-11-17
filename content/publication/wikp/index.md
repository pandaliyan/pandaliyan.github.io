---
title: "Words Worth a Thousand Pictures: Measuring and Understanding Perceptual Variability in Text-to-Image Generation"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Raphael Tang 
- Crystina Zhang
- Lixinyu Xu 
- Yao Lu
- admin
- Pontus Stenetorp
- Jimmy Lin 
- Ferhan Ture


# Author notes (optional)
author_notes:
- ""
- ""

date: "2024-11-16T00:00:00Z"
# doi: "10.18653/v1/2020.findings-emnlp.12"

# Schedule page publish date (NOT publication's date).
publishDate: "2024"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "In *EMNLP 2024 main*"
publication_short: "In *EMNLP 2024 main (Outstanding Paper Award)*"

abstract: "Diffusion models are the state of the art in text-to-image generation, but their perceptual variability remains understudied. In this paper, we examine how prompts affect image variability in black-box diffusion-based models. We propose W1KP, a human-calibrated measure of variability in a set of images, bootstrapped from existing image-pair perceptual distances. Current datasets do not cover recent diffusion models, thus we curate three test sets for evaluation. Our best perceptual distance outperforms nine baselines by up to 18 points in accuracy, and our calibration matches graded human judgements 78% of the time. Using W1KP, we study prompt reusability and show that Imagen prompts can be reused for 10-50 random seeds before new images become too similar to already generated images, while Stable Diffusion XL and DALL-E 3 can be reused 50-200 times. Lastly, we analyze 56 linguistic features of real prompts, finding that the prompt's length, CLIP embedding norm, concreteness, and word senses influence variability most. As far as we are aware, we are the first to analyze diffusion variability from a visuolinguistic perspective."

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: [Multimodal]

# Display this page in the Featured widget?
featured: true

math: true

# Custom links (uncomment lines below)
links:
- name: Website
  url: http://w1kp.com/

url_pdf: 'https://aclanthology.org/2024.emnlp-main.311'

# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []
# - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""

---
