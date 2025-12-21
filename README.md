# Website Maintenance Guide


## Installing Jekyll

This is a Jekyll website. To run it in your computer, I highly recommend
installing Jekyll using conda. 

First, create a conda environment

```bash
  conda create -n jekyll_env python
  conda activate jekyll_env
```

Install the dependencies:

```bash
  conda install -c conda-forge c-compiler compilers cxx-compiler ruby
  gem install jekyll bundler
```

You can then run the website locally using 

```bash
  jekyll serve
```

## Key pages

The key pages of the website are located in `_pages/`. There are currently five
such pages:

- `main.html` 
- `people.html`
- `joinus.md`
- `press.html`
- `publications.html`

## Update lab members

To add new members, create a new `.md` file on `my_collections/_members`. 

Please name the file `{name}.md`, e.g., `manoel.md`. This is an example file:

```
---
name: 'Hayoung Jung'
title: 'PhD Student'
email: 'hayoung@cs.princeton.edu'
link: 'https://hayoungjung.me/'
comment: 'Co-advised with Aleksandra Korolova'
photo: 'hayoung.jpg'
---
```

## Update publications

To add any publications, create a new `.md` file on 
`my_collections/_publications`. 

Please name the file  `{year}_{whatever}.md`, e.g., `2025_msr.md`. This is an 
example file:


```md
---
title: 'YouNiverse: Large-Scale Channel and Video Metadata from English-Speaking YouTube'
authors:
    - Manoel Horta Ribeiro
    - Robert West

year: 2021

conf: 'ICWSM'

links:
  - {"name": "📜 Paper", "content": "https://ojs.aaai.org/index.php/ICWSM/article/view/18125/17928"}
  - {"name": "📄 Pre-print", "content": "https://arxiv.org/abs/2012.10378"}
  - {"name": "🔗️ Code", "content": "https://github.com/epfl-dlab/YouNiverse/"}
  - {"name":"🗄️ Data", "content": "https://zenodo.org/record/4650046"}
  - {"name": "🌐 Blog", "content": "https://dlab.epfl.ch/2021-05-19-YouNiverse/"}
  - {"name": "▶️ Slides", "content": "https://docs.google.com/presentation/d/1jVhJ87ezcXh-hQKvbFiGSn1r-UP1nxfB7E8lpACeJZg/edit?usp=sharing"}
  - {"name": "📹 Presentation", "content":"https://www.youtube.com/watch?v=pqEodXPP3hI"}
  - {"name": "🐦 Tweet", "content":"https://twitter.com/manoelribeiro/status/1341082283223240706"}

name_file: '2021_yt'
---
```

Fields are mostly self-explanatory. Yet, note that links is pretty generic! 
You can have any kind of content there. Note also that `name_file` is
deprecated, you don't need to add it.


## Update press

To add any media coverage, create a new `.md` file on `my_collections/_media`. 

Please name the file `{year}_{outlet alias}.md`, e.g., `2023_bloomberg.md`. This is an example file:

```

---
title: "The Ghost in the Machine Shouldn’t Be AI"

year: 2023

venue: "Bloomberg"

link: "https://www.bloomberg.com/opinion/articles/2023-06-19/chatgpt-on-mechanical-turk-teaching-ai-with-ai-comes-with-risks?srnd=premium"

archive: "https://web.archive.org/web/20230703223624/https://www.bloomberg.com/opinion/articles/2023-06-19/chatgpt-on-mechanical-turk-teaching-ai-with-ai-comes-with-risks?srnd=premium"

related_paper: 'Artificial Artificial Artificial Intelligence: Crowd Workers Widely Use Large Language Models for Text Production Tasks'

---
```

The fields are self-explanatory, but note that the string under `related_paper`
should match exactly the title of a publication in 
`my_collections/_publications`, so that it is rendered there.

As a convention, if the newspiece is not in English, please include the flag of
the country of origin with an emoji besides the venue. For instance:

```
"venue": "🇧🇷 Folha de São Paulo"
```