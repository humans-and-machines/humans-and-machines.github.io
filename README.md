# Website Maintenance Guide

TODO

## Update lab members

To add any media coverage, create a new `.md` file on `members/_media`. 

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

To add any publications coverage, create a new `.md` file on 
`my_collections/_publications`. 

## Update media

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
"venue": "🇧🇷Folha de São Paulo"
```