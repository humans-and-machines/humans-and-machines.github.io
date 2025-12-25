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
- `press.html`
- `publications.html`
- `joinus.md`

Below, we describe how to handle each such pages

## `main.html` — Add events

You can add new noteworthy events by adding a row to `_data/news.yml`. E.g.,

```yaml
    - {
        "date": "2025-11-10",
        "text": "🏆 Manoel was commended for his teaching at Princeton!",
        "link": "https://engineering.princeton.edu/news/2025/11/10/faculty-commended-outstanding-teaching-8",
      }
```

What are noteworthy events? Any of the following:

- Awards / Grants
- Papers accepted at conferences
- Noteworthy lab events (e.g., someone new joined, got a job, got a dog).


## `people.html` — Update lab members

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

## Update publications — `publications.html`

To add any publications, create a new `.md` file on 
`my_collections/_publications`. 

Please name the file  `{year}_{whatever}.md`, e.g., `2025_msr.md`. This is an 
example file:


```md
---
title: 'The AI Review Lottery: Widespread AI-Assisted Peer Reviews Boost Paper Scores and Acceptance Rates'

authors:

  - Giuseppe Russo
  - Manoel Horta Ribeiro
  - Tim Reuben Davidson
  - Veniamin Veselovsky
  - Robert West
  
year: 2025

conf: 'CSCW'

awards: ['🏆 Best Paper Honorable Mention Award']

links:
  
  - {"name": "📜 Paper", "content": "https://dl.acm.org/doi/abs/10.1145/3757667"}
  - {"name": "📄 Pre-print", "content": "https://arxiv.org/abs/2405.02150"}
  - {"name": "🐦 Tweet", "content": "https://x.com/manoelribeiro/status/1787512594661572878"}

---
```

Fields are mostly self-explanatory. Note that links is pretty generic! 
You can have any kind of content there. Check the publication page to see 
what is typically shared. 

## `press.html` — Update press 

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

