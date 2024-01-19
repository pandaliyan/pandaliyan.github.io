---
title: "The Role of Data Curation in Image Captioning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin 
- Jonas F Lotz
- Chen Qiu
- Desmond Elliott


# Author notes (optional)
author_notes:
- ""
- ""

date: "2024-01-19T00:00:00Z"
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: "2024"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "*EACL* 2024 (to appear)"
publication_short: "*EACL 2024* (to appear)"

abstract: "Image captioning models are typically trained by treating all samples equally, neglecting to account for mismatched or otherwise difficult data points. In contrast, recent work has shown the effectiveness of training models by scheduling the data using curriculum learning strategies. This paper contributes to this direction by actively curating difficult samples in datasets *without* increasing the total number of samples. 
    We explore the effect of using three data curation methods within the training process: complete removal of an sample, caption replacement, or image replacement via a text-to-image generation model. Experiments on the Flickr30K and COCO datasets with the BLIP and BEiT-3 models demonstrate that these curation methods do indeed yield improved image captioning models, underscoring their efficacy."

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: [Multimodal]

# Display this page in the Featured widget?
featured: true

math: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: /publication/sd-synth2023/wli_EACL_2024_preprint.pdf
# url_code: ''
# url_dataset: ''
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
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
